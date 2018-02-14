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

# 시스템 보고서 작성
{: #cp_compuschrootkit}

Chrootkit 도구를 사용하여 시스템 보고서를 스캔하고 작성하고 이메일을 발송할 수 있습니다.
{:shortdesc}

Chrootkit 도구를 사용하려면 서버에 관리자로 먼저 SSH를 설정하십시오. 이미 사용 안함으로 설정되어야 하는 telnet을 사용하지 마십시오. 그런 다음, 다음 단계를 완료하십시오. 

1. 루트 디렉토리로 변경하십시오.   

  ```
  su -
  ```
  {: pre}

2. 다음 명령을 실행하십시오.

  ```
  wget ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.tar.gz
  ```
  {: pre}

3. 보안을 위해 다운로드의 MD5 SUM을 확인하십시오.<br/

  ```
  ftp://ftp.pangeia.com.br/pub/seg/pac/chkrootkit.md5
  md5sum chkrootkit.tar.gz
  ```
  {: pre}

4. 다음 명령을 사용하여 tarball을 언팩하십시오. <br/>

  ```
  tar xvzf chkrootkit.tar.gz
  ```
  {: pre}

5. 작성된 디렉토리로 변경하십시오. 

  ```
  cd chkrootkit*
  ```
  {: pre}

6. 다음 명령을 실행하여 결과를 컴파일하십시오.

  ```
  make sense
  ```
  {: pre}

7. chkrootkit를 사용하려면 다음 명령을 입력하십시오. 

  ```
  ./chkrootkit
  ```
  {: pre}

전체 chkrootkit 도구 출력은 `not found` 또는 `not infected`여야 합니다.

*`bindshell`... INFECTED (PORTS: 465) 확인 중*이 표시되고 PortSentry, klaxon 또는 사용되지 않는 포트로 자체 바인드하는 다른 프로그램을 실행하는 경우 chkrootkit는 bindshell 테스트(포트 114/tcp, 465/tcp, 511/tcp, 1008/tcp, 1524/tcp, 1999/tcp, 3879/tcp, 4369/tcp, 5665/tcp, 10008/tcp, 12321/tcp, 23132/tcp, 27374/tcp, 29364/tcp, 31336/tcp, 31337/tcp, 45454/tcp, 47017/tcp, 47889/tcp, 60001/tcp)에 거짓 긍정(false positive)을 제공할 가능성이 있습니다.
{: tip}

8. 디렉토리(`cd ..`)를 변경하고 .gz 파일을 제거하십시오.   

  ```
  rm chkrootkit.tar.gz
  ```
  {: pre}

## 일별 자동화된 스캔 전송
{: #cp_chrootkitdaiautscan}

보고서를 이메일로 발송하는 일별 자동화된 시스템 스캔을 설정하려면 다음 단계를 수행하십시오. 

1. SSH에서 다음 명령을 실행하십시오. 

  ```
  pico /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

2. 새 파일에 다음 행을 추가하십시오. 

  ```
  #!/bin/bash<br/>
  cd /yourinstallpath/chkrootkit-0.42b/<br/>
  ./chkrootkit | mail -s "Daily chkrootkit from Servername" admin@youremail.com
  ```
  {: pre}

3. `yourinstallpath`를 Chkrootkit를 언팩한 실제 경로로 대체하십시오. 
4. `Servername`을 실행 중이어서 발생 위치를 알고 있는 서버로 변경하십시오. 
5. `admin@youremail.com`을 스크립트에서 이메일을 발송할 실제 이메일 주소로 변경하십시오. 
6. 다음 명령을 사용하여 SSH에 파일을 저장하십시오. 

  ```
  Ctrl+X then type Y
  ```
  {: pre}

7. 실행하려면 파일 권한을 변경하십시오. 

  ```
  chmod 755 /etc/cron.daily/chkrootkit.sh
  ```
  {: pre}

8.  선택적으로, SSH에서 수동으로 테스트 보고서를 실행하여 작동 방식을 볼 수 있습니다. 

  ```
  cd /etc/cron.daily/
  ./chkrootkit.sh
  ```
  {: pre}

이제 수동으로 수행할 필요 없이 매일 보고서가 포함된 이메일을 받게 됩니다. 
