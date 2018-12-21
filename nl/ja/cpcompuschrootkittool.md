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

# システム・レポートの作成
{: #cp_compuschrootkit}

Chrootkit ツールを使用して、システム・レポートのスキャン、作成、および E メール送信を行うことができます。
{:shortdesc}

Chrootkit ツールを使用するには、最初に管理者として SSH でサーバーに接続します。 telnet は使用しないでください (既に使用不可になっています)。 次に、以下の手順を使用します。

1. ルート・ディレクトリーに移動します。  

  ```
  su -
  ```
  {: pre}

2. 次のコマンドを実行します。

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. セキュリティーのため、ダウンロードの MD5 SUM をチェックします。<br/>

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. 次のコマンドを使用して tarball を解凍します。<br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. 作成されたディレクトリーに移動します。

  ```
  cd chkrootkit*
  ```
  {: pre}

6. 次のコマンドを実行して、結果をコンパイルします。

  ```
  make sense
  ```
  {: pre}

7. chkrootkit を使用するには、次のコマンドを入力します。

  ```
  ./chkrootkit
  ```
  {: pre}

chkrootkit ツールの出力は `not found` または `not infected` のみである必要があります。

*Checking `bindshell`... INFECTED (PORTS: 465)* が表示され、かつ、PortSentry、klaxon、または未使用ポートに自身をバインドする他のプログラムが実行されている場合、chkrootkit の bindshell テストで誤検出の可能性があります (ポート 114/tcp、465/tcp、511/tcp、1008/tcp、1524/tcp、1999/tcp、3879/tcp、4369/tcp、5665/tcp、10008/tcp、12321/tcp、23132/tcp、27374/tcp、29364/tcp、31336/tcp、31337/tcp、45454/tcp、47017/tcp、47889/tcp、60001/tcp)。
{: tip}

8. ディレクトリーを変更し (`cd ..`)、.gz ファイルを削除します。  

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## 日次自動スキャンの送信
{: #cp_chrootkitdaiautscan}

レポートを E メール送信する日次自動システム・スキャンをセットアップするには、以下の手順を使用します。

1. SSH にいる間に次のコマンドを実行します。

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. 新規ファイルに次の行を追加します。

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. `yourinstallpath` を、Chkrootkit を解凍した実際のパスに置き換えます。
4. `Servername` を、実行しているサーバーに変更して、送信元が分かるようにします。
5. `admin@youremail.com` を、このスクリプトが E メールを送信する先の実際の E メール・アドレスに変更します。
6. 次のコマンドを使用して、ファイルを SSH で保存します。

  ```
  Ctrl+X の後で Y を入力
  ```
  {: pre}

7. 実行できるようにファイル許可を変更します。

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  オプションで、SSH でテスト・レポートを手動で実行して、どのようなものかを確認できます。

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

これで、レポートを毎日 E メールで受信するようにすべて設定されたので、手動で実行する必要はありません。
