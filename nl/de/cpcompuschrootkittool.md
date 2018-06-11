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

# Systemberichte erstellen
{: #cp_compuschrootkit}

Mit dem Tool 'Chrootkit' können Sie Systemberichte überprüfen, erstellen und per E-Mail senden.
{:shortdesc}

Melden Sie sich zur Verwendung des Tools 'Chrootkit' zunächst über eine SSH-Verbindung als Administrator bei Ihrem Server an. Verwenden Sie nicht Telnet, das bereits inaktiviert sein sollte. Gehen Sie anschließend wie folgt vor:

1. Wechseln Sie in das Stammverzeichnis:  

  ```
  su -
  ```
  {: pre}

2. Führen Sie den folgenden Befehl aus:

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. Überprüfen Sie den Wert für MD5 SUM des Downloads für die Sicherheit:<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. Entpacken Sie die TAR-Datei mit dem folgenden Befehl:<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. Wechseln Sie in das hierdurch erstellte Verzeichnis:

  ```
  cd chkrootkit*
  ```
  {: pre}

6. Kompilieren Sie die Ergebnisse mit dem folgenden Befehl:

  ```
  make sense
  ```
  {: pre}

7. Geben Sie zur Verwendung von 'chkrootkit' den folgenden Befehl ein:

  ```
  ./chkrootkit
  ```
  {: pre}

Alle Ausgaben des Tools 'chkrootkit' sollten `not found` oder `not infected` lauten.

Falls *Checking `bindshell`... INFECTED (PORTS: 465)* angezeigt wird und Sie PortSentry, klaxon oder ein anderes Programm ausführen, das sich selbst an nicht belegte Ports bindet, gibt 'chkrootkit' wahrscheinlich einen Fehlalarm für den Bindshell-Test aus (Ports 114/tcp, 465/tcp, 511/tcp, 1008/tcp, 1524/tcp, 1999/tcp, 3879/tcp, 4369/tcp, 5665/tcp, 10008/tcp, 12321/tcp, 23132/tcp, 27374/tcp, 29364/tcp, 31336/tcp, 31337/tcp, 45454/tcp, 47017/tcp, 47889/tcp, 60001/tcp).
{: tip}

8. Wechseln Sie das Verzeichnis (`cd ..`) und entfernen Sie die Datei '.gz':  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## Automatisierte tägliche Scans senden
{: #cp_chrootkitdaiautscan}

Um einen automatisierten täglichen Systemscan zu konfigurieren, der Ihnen einen Bericht per E-Mail sendet, gehen Sie folgendermaßen vor:

1. Führen Sie in SSH den folgenden Befehl aus:

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. Fügen Sie die folgende Zeile zu der neuen Datei hinzu:

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. Ersetzen Sie `yourinstallpath` durch den tatsächlichen Pfad, unter dem Sie 'Chkrootkit' entpackt haben.
4. Ändern Sie `Servername` in den Server, den Sie ausführen, damit Sie den Ursprung kennen.
5. Ändern Sie `admin@youremail.com` in Ihre tatsächliche E-Mail-Adresse, an die das Script die E-Mail an Sie senden soll.
6. Speichern Sie die Datei in SSH mit dem folgenden Befehl:

  ```
  Geben Sie Strg+X und anschließend Y ein.
  ```
  {: pre}

7. Ändern Sie die Dateiberechtigung für die Ausführung:

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  Optional können Sie manuell einen Testbericht in SSH erstellen, um dessen Darstellung anzuzeigen:

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

Sie haben hiermit den täglichen Empfang einer E-Mail mit dem Bericht konfiguriert und müssen den Bericht nicht manuell ausführen.
