---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-06"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Creazione dei report di sistema
{: #cp_compuschrootkit}

Puoi utilizzare lo strumento Chrootkit per eseguire la scansione, creare e inviare via email i report di sistema.
{:shortdesc}

Per utilizzare lo strumento Chrootkit, per prima cosa accedi tramite SSH al tuo server come amministratore. Non utilizzare telnet, che dovrebbe essere già disabilitato. Completa quindi la seguente procedura:

1. Passa alla directory root:  

  ```
  su -
  ```
  {: pre}

2. Immetti il seguente comando:

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. Controlla il valore MD5 SUM del download per sicurezza:<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. Decomprimi il tarball utilizzando il seguente comando:<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. Passa alla directory creata:

  ```
  cd chkrootkit*
  ```
  {: pre}

6. Compila i risultati immettendo il seguente comando:

  ```
  make sense
  ```
  {: pre}

7. Per utilizzare chkrootkit, immetti il seguente comando:

  ```
  ./chkrootkit
  ```
  {: pre}

Tutto ciò che viene emesso dallo strumento chkrootkit deve essere `not found` o `not infected`.

Se visualizzi *Checking `bindshell`... INFECTED (PORTS: 465)* e stai eseguendo PortSentry, klaxon o un altro programa che si collega a porte non utilizzate, è probabile che chkrootkit ti dia un falso positivo nel test bindshell (porte 114/tcp, 465/tcp, 511/tcp, 1008/tcp, 1524/tcp, 1999/tcp, 3879/tcp, 4369/tcp, 5665/tcp, 10008/tcp, 12321/tcp, 23132/tcp, 27374/tcp, 29364/tcp, 31336/tcp, 31337/tcp, 45454/tcp, 47017/tcp, 47889/tcp, 60001/tcp).
{: tip}

8. Modifica la directory (`cd ..`) e rimuovi il file .gz:  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## Invio di scansioni automatiche giornaliere
{: #cp_chrootkitdaiautscan}

Per configurare una scansione del sistema automatizzata giornaliera che ti invii un report via e-mail, utilizza la seguente procedura:

1. Mentre utilizzi SSH, immetti il seguente comando:

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. Aggiungi la seguente riga al nuovo file:

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. Sostituisci `yourinstallpath` con il percorso reale in cui hai decompresso Chkrootkit.
4. Modifica `Servername` con il server che stai utilizzando in modo da sapere da dove proviene.
5. Modifica `admin@youremail.com` con il tuo indirizzi e-mail reale dove vuoi che lo script ti invii una e-mail.
6. Utilizza il seguente comando per salvare il file in SSH:

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. Modifica le autorizzazioni del file per utilizzarlo.

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  Facoltativamente, puoi eseguire un report di test manualmente in SSH per vedere come appare:

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

È tutto pronto per ricevere un'e-mail giornaliera con il report in modo da non doverlo eseguire manualmente.
