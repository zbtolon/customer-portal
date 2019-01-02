---

copyright:

  years: 1994, 2018

lastupdated: "2017-10-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Criando relatórios do sistema
{: #cp_compuschrootkit}

É possível usar a ferramenta Chrootkit para varrer, criar e enviar e-mail de relatórios do sistema.
{:shortdesc}

Para usar a ferramenta Chrootkit, primeiro execute o SSH como o administrador para seu servidor. Não use telnet, que já deve estar desativado. Em seguida, use as etapas a seguir:

1. Mude para o diretório raiz:  

  ```
  su -
  ```
  {: pre}

2. Execute o seguinte comando:

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. Verifique o MD5 SUM do download para security:<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. Descompacte o tarball usando o comando a seguir:<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. Mude para o diretório que ele criou:

  ```
  cd chkrootkit*
  ```
  {: pre}

6. Compile os resultados executando o comando a seguir:

  ```
  make sense
  ```
  {: pre}

7. Para usar o chkrootkit, insira o comando a seguir:

  ```
  ./chkrootkit
  ```
  {: pre}

Tudo o que a ferramenta chkrootkit emite como saída deve ser `not found` ou `not infected`.

Se você vir *Verificando `bindshell`... INFECTADAS (PORTAS: 465)* e estiver executando o PortSentry, o klaxon ou outro programa que se ligue a portas não usadas, o chkrootkit provavelmente lhe dará um falso positivo no teste de bindshell (portas 114/tcp, 465/tcp, 511/tcp, 1008/tcp, 1524/tcp, 1999/tcp, 3879/tcp, 4369/tcp, 5665/tcp, 10008/tcp, 12321/tcp, 23132/tcp, 27374/tcp, 29364/tcp, 31336/tcp, 31337/tcp, 45454/tcp, 47017/tcp, 47889/tcp, 60001/tcp).
{: tip}

8. Mude o diretório (`cd ..`) e remova o arquivo .gz:  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## Enviando varreduras automatizadas diariamente
{: #cp_chrootkitdaiautscan}

Para configurar uma varredura do sistema automatizada que envia diariamente e-mails de um relatório, use as etapas a seguir:

1. Enquanto está no SSH, execute o comando a seguir:

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. Inclua a linha a seguir no novo arquivo:

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. Substitua `yourinstallpath` pelo caminho real no qual você descompactou o Chkrootkit.
4. Mude `Servername` para o servidor que você está executando para que saiba de onde ele está vindo.
5. Mude `admin@youremail.com` para seu endereço de e-mail real para o qual deseja que o script envie o e-mail.
6. Use o comando a seguir para salvar o arquivo em SSH:

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. Mude as permissões do arquivo para executá-lo:

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  Opcionalmente, é possível executar um relatório de teste manualmente no SSH para ver como fica:

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

Está tudo pronto para receber um e-mail diário com o relatório para que você não precise executá-lo manualmente.
