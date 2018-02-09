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

# Creación de informes del sistema
{: #cp_compuschrootkit}

Puede utilizar la herramienta Chrootkit para explorar, crear y enviar por correo electrónico los informes del sistema.
{:shortdesc}

Para utilizar la herramienta Chrootkit, en primer lugar conéctese por SSH como administrador a su servidor. No utilice telnet, que ya debería estar inhabilitado. A continuación, utilice los pasos siguientes:

1. Vaya al directorio raíz:  

  ```
  su -
  ```
  {: pre}

2. Ejecute el mandato siguiente:

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. Compruebe el MD5 SUM de la descarga por seguridad:<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. Desempaquete el fixpack comprimido mediante este mandato:<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. Vaya al directorio que ha creado:

  ```
  cd chkrootkit*
  ```
  {: pre}

6. Compile los resultados ejecutando el mandato siguiente:

  ```
  make sense
  ```
  {: pre}

7. Para utilizar chkrootkit, escriba el siguiente mandato:

  ```
  ./chkrootkit
  ```
  {: pre}

Todo lo que la herramienta chkrootkit da como resultado debería ser `no encontrado` o `no infectado`.

Si ve *Checking `bindshell`... INFECTED (PORTS: 465)* y está ejecutando PortSentry, klaxon, u otro programa que se enlaza a los puertos no utilizados, chkrootkit es probable que le dé un falso positivo en la prueba bindshell (puertos 114/tcp, 465/tcp, 511/tcp, 1008/tcp, 1524/tcp, 1999/tcp, 3879/tcp, 4369/tcp, 5665/tcp, 10008/tcp, 12321/tcp, 23132/tcp, 27374/tcp, 29364/tcp, 31336/tcp, 31337/tcp, 45454/tcp, 47017/tcp, 47889/tcp, 60001/tcp).
{: tip}

8. Cambie el directorio (`cd ..`) y elimine el archivo .gz:  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## Envío de exploraciones automáticas diarias
{: #cp_chrootkitdaiautscan}

Para configurar una exploración del sistema automatizada diaria que le envíe por correo electrónico un informe, utilice los pasos siguientes:

1. Mientras esté en SSH, ejecute el mandato siguiente:

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. Añada la línea siguiente al archivo nuevo:

  ```
#!/bin/bash
<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. Sustituya `yourinstallpath` por la vía de acceso real donde ha desempaquetado Chkrootkit.
4. Cambie `Servername` por el servidor que está ejecutando, para que sepa de dónde viene.
5. Cambie `admin@youremail.com` por la dirección de correo electrónico real donde desea que el script le escriba.
6. Utilice el mandato siguiente para guardar el archivo en SSH:

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. Cambie los permisos de archivo para ejecutarlo:

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  Opcionalmente, puede ejecutar un informe de prueba manualmente en SSH para ver qué aspecto tiene:

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

Ya está listo para recibir un correo electrónico diario con el informe para que no tenga que ejecutarlo manualmente.
