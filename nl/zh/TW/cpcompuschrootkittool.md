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

# 建立系統報告
{: #cp_compuschrootkit}

您可以使用 Chrootkit 工具來掃描、建立以及以電子郵件寄送系統報告。
{:shortdesc}

若要使用 Chrootkit 工具，請先以 admin 身分透過 SSH 進入伺服器。請不要使用應該已停用的 Telnet。然後，使用下列步驟：

1. 切換至根目錄：  

  ```
  su -
  ```
  {: pre}

2. 請執行下列指令：

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. 檢查下載的 MD5 SUM 的安全性：<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. 使用下列指令來解壓縮 Tarball：<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. 切換至它建立的目錄：

  ```
  cd chkrootkit*
  ```
  {: pre}

6. 執行下列指令來編譯結果：

  ```
  make sense
  ```
  {: pre}

7. 若要使用 chkrootkit，請輸入下列指令：

  ```
  ./chkrootkit
  ```
  {: pre}

chkrootkit 工具所輸出的所有內容都應該是 `not found` 或 `not infected`。

如果您看到 *Checking `bindshell`... INFECTED (PORTS: 465)*，而且正在執行 PortSentry、klaxon 或另一個將它自己連結至未用埠的程式，則 chkrootkit 可能會對 bindshell 測試提供誤判（埠 114/tcp、465/tcp、511/tcp、1008/tcp、1524/tcp、1999/tcp、3879/tcp、4369/tcp、5665/tcp、10008/tcp、12321/tcp、23132/tcp、27374/tcp、29364/tcp、31336/tcp、31337/tcp、45454/tcp、47017/tcp、47889/tcp、60001/tcp）。
{: tip}

8. 切換目錄 (`cd ..`)，並移除 .gz 檔案：  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## 傳送每日自動掃描
{: #cp_chrootkitdaiautscan}

若要設定以電子郵件寄送報告的每日自動系統掃描，請使用下列步驟：

1. 處於 SSH 時，請執行下列指令：

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. 將下列這幾行新增至新檔案：

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. 將 `yourinstallpath` 取代為已解壓縮 Chkrootkit 的實際路徑。
4. 將 `Servername` 變更為您正在執行的伺服器，讓您知道它的來源。
5. 將 `admin@youremail.com` 變更為您要 Script 寄送電子郵件的實際電子郵件位址。
6. 使用下列指令，以將檔案儲存至 SSH：

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. 變更檔案許可權，以執行檔案：

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  您可以選擇在 SSH 中手動執行測試報告，以查看其內容：

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

您已設為接收含報告的每日電子郵件，因此不需要手動執行。
