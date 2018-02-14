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

# 创建系统报告
{: #cp_compuschrootkit}

您可以使用 Chrootkit 工具来扫描和创建系统报告以及通过电子邮件发送系统报告。
{:shortdesc}

要使用 Chrootkit 工具，请首先以管理员身份通过 SSH 登录到服务器。不要使用 Telnet，此项应该已禁用。然后，使用以下步骤：

1. 切换到 root 目录：  

  ```
  su -
  ```
  {: pre}

2. 运行以下命令：

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. 检查下载的 MD5 SUM 以确保安全性：<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. 使用以下命令解包 tarball：<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. 切换到它所创建的目录：

  ```
  cd chkrootkit*
  ```
  {: pre}

6. 通过运行以下命令来编译结果：

  ```
  make sense
  ```
  {: pre}

7. 要使用 chkrootkit，请输入以下命令：

  ```
  ./chkrootkit
  ```
  {: pre}

chkrootkit 工具输出的所有内容都应该是 `not found` 或 `not infected`。

如果看到 *Checking `bindshell`... INFECTED (PORTS: 465)*，并且运行的是 PortSentry、klaxon 或将自身绑定到未使用的端口的其他程序，那么 chkrootkit 很可能会针对 bindshell 测试提供误报（端口 114/tcp、465/tcp、511/tcp、1008/tcp、1524/tcp、1999/tcp、3879/tcp、4369/tcp、5665/tcp、10008/tcp、12321/tcp、23132/tcp、27374/tcp、29364/tcp、31336/tcp、31337/tcp、45454/tcp、47017/tcp、47889/tcp 和 60001/tcp）。
{: tip}

8. 切换目录 (`cd ..`) 并除去 .gz 文件：  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## 发送每天自动扫描
{: #cp_chrootkitdaiautscan}

要设置通过电子邮件向您发送报告的每天自动系统扫描，请使用以下步骤：

1. 在 SSH 中运行以下命令：

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. 向新文件添加以下行：

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. 将 `yourinstallpath` 替换为 Chkrootkit 实际解包路径。
4. 将 `Servername` 更改为要运行的服务器，以便您知道其来源。
5. 将 `admin@youremail.com` 更改为您希望接收脚本发送的电子邮件的实际电子邮件地址。
6. 使用以下命令在 SSH 中保存文件：

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. 更改文件许可权以加以运行：

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  （可选）可以在 SSH 中手动运行测试报告来查看其内容：

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

至此您已全部设置好，每天将通过电子邮件接收报告，因此不必手动运行。
