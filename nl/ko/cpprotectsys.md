---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-04"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 시스템 보호
{: #customerportal_protsys}

시스템 보호를 통해 불필요한 인터럽트 없이 시스템을 원활하게 실행할 수 있습니다. 

## 사설 네트워크 사용
{: #cp_bpuseprivnet}

{{site.data.keyword.BluSoftlayer_notm}} 인프라 사설 네트워크 사용하여 가능한 가장 안전한 환경에서 디바이스를 관리할 수 있습니다. 가능하면 시스템이 사설 네트워크를 통해 통신하도록 VPN 연결을 사용하여 디바이스와 상호작용하고 사설 네트워크 범위를 사용 가능하도록 설정하십시오. 사설 네트워크에 액세스하려면 [사용자 목록 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}에서
사용자의 VPN 액세스를 편집하십시오. [가상 사설망(VPN) ![외부 링크 아이콘](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} 지시사항을 사용하여
여러 VPN 옵션 중 하나에 연결하십시오. 

### RDP, SSH 또는 제어 포트를 공용 네트워크에 두지 않음
{: #cp_bpnordpsshcponpubnet}

공용 네트워크는 여러가지 면에서 장점이 있지만, 개방형 포트를 통해 공용 네트워크에 사용 가능하도록 둘 경우 시스템이 취약한 상태가 될 수 있는 일부 요소가 있습니다. 공용 네트워크에서 RDP를 사용하지 않고 SSH를 제한하여 자체적으로 보호하십시오.
이 서비스가 공용 네트워크에서 사용 가능해야 하는 경우 RDP 또는 SSH를 사용자 정의 포트 번호로 이동하는 것을 고려해보십시오. 

## 정기 백업을 통한 데이터 보호
{: #cp_bpsafedataregback}

{{site.data.keyword.BluSoftlayer_notm}} 인프라는 드라이브 장애 또는 사용자 오류 발생 시 데이터를 검색할 수 있도록
다중 백업 솔루션을 제공합니다. 백업 솔루션에는 현재 NAS, EVault Backup 및 R1Soft CDP가 포함되며, 모두 다양한 스토르지 옵션에서 사용할 수 있습니다. 각 백업 솔루션의 자세한 정보는
[스토리지 ![외부 링크 아이콘](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} 페이지를 확인하십시오. 

### 중복성이 있다고 간주하지 않음(수행하는 작업을 알고 있음)
{: #cp_bpknowredundant}

{{site.data.keyword.BluSoftlayer_notm}} 인프라는 이중 경로, 이중 전원 공급 및 RAID 구성을 포함하여 여러 추가 기능 중복을 제공합니다. 중복 환경에서 작업하고 장애 발생 시 보호될 수 있도록 하나 이상의 기능을 프로비저닝했는지 확인하십시오. 

### OS를 다시 로드하기 전에 사용자의 정보가 백업되었는지 확인함
{: #cp_bpnoperfOSwobackupconf}

운영 체제를 다시 로드하면 디바이스의 하드 드라이브에서 모든 데이터가 제거됩니다. OS 다시 로드를 시작하기 전에 정보를 백업하고 백업 성공을 확인하여 정보가 유실되지 않도록 하십시오. OS 다시 로드가 완료된 후 유실된 정보를 검색할 수 없습니다. 

## ASM(Aaptec Storage Manager) 제거 안 함
{: #cp_bpsupdontremovasm}

 {{site.data.keyword.BluSoftlayer_notm}} 인프라는 ASM을 사용하여 RAID 배열 상태를 모니터합니다. 이 소프트웨어를 삭제하는 경우 지원 팀에서 디바이스를 모니터할 수 업습니다. 디바이스에서 ASM을 제거하면 디바이스에 대한 RAID 장애 알림을 사용할 수 없고 자동 알림 시스템을 통한 장애 알림을 받을 수 없게 됩니다. 
