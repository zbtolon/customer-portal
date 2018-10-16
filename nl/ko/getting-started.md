---

copyright:

  years: 1994, 2018

lastupdated: "2018-10-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 시작하기 튜토리얼
{: #getting-started}

이 튜토리얼에서는 인프라 리소스 주문을 시작하고 관리할 수 있도록 SoftLayer 계정을 시작하고 실행하기 위한 프로세스에 대해 설명합니다.
{:shortdesc}

## 시작하기 전에
{: #prereqs}

[{{site.data.keyword.Bluemix}} 계정 ![외부 링크 아이콘](../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net/){:new_window}이 필요합니다. IBM ID 인증 정보를 사용하여 고객 포털에 로그인하십시오. 대부분의 신규 사용자는 인증에 [IBM ID](/docs/account/softlayerlink.html#switchtoIBMid)를 사용합니다.

인증용 IBM ID를 사용하여 계정에 로그인하지 않는 경우에는 고유 {{site.data.keyword.BluSoftlayer_notm}} 인프라 인증 정보를 사용하여 고객 포털에 로그인하십시오.
{: tip}

## 1단계. 계정 설정
{: #account-setup}

계정을 설정하면 계정 연락처 정보와 청구 세부사항 확인이 포함됩니다.
 * 회사 담당자 세부사항을 확인하려면 **계정** > **관리** > **회사 담당자**로 이동하십시오. 계정의 회사 담당자 정보는 계정의 문제 또는 변경에 대한 알림을 제공하는 데 사용됩니다.
 * 회사 프로파일 세부사항을 확인하려면 **계정** > **관리** > **회사 프로파일**로 이동하십시오. 회사 프로파일 정보는 기본 계정 소유자에 대한 세부사항을 포함합니다.
 * 청구 세부사항을 확인하려면 **계정** > **청구** > **결제 방법**으로 이동하십시오. 월별 결제 방법은 계정과 연관된 지불 금액에 대해 주기적으로 비용이 청구되는 신용 카드입니다.

## 2단계. 사용자 추가 및 권한 지정
{: #users-permissions}

사용자를 계정에 추가하고 초기 권한을 설정하려면 **계정** > **사용자**로 이동하십시오.
 * 지정한 특정 권한을 기반으로 계정에서 플랫폼 및 인프라 리소스 모두에 사용자를 초대하려면 **사용자 초대**를 클릭하십시오. 그러면 {{site.data.keyword.Bluemix_notm}} Identity and Access Management(Tivoli Information Archive Manager) UI로 이동하여 사용자를 초대하고 액세스를 지정할 수 있습니다. 자세한 정보는 [사용자 초대 및 액세스 지정](/docs/iam/iamuserinv.html)을 참조하십시오.
 * VPN 액세스가 있는 사용자만 추가하려면 **VPN 전용 사용자 추가**를 클릭하십시오. 개인 정보를 입력하려면 포털 권한을 설정하고 사용자를 위해 디바이스 액세스를 설정하십시오.

초기 초대에서 인프라 권한을 설정하려면 보기 전용, 기본 사용자, 수퍼유저 중에서 하나의 권한 세트를 선택하십시오. 사용자가 초대를 수락하면 포털 권한을 편집하여 액세스를 사용자 정의할 수 있습니다. 자세한 정보는 [인프라 권한](/docs/iam/infrastructureaccess.html)을 참조하십시오.
{: tip}

## 3단계. {{site.data.keyword.Bluemix_notm}} 인프라 사설 네트워크
{: #enable-private-network}

{{site.data.keyword.Bluemix_notm}} 인프라 사설 네트워크는 사용자와 디바이스에 무료로 제공됩니다. 사설 네트워크의 대역폭은 측정되지 않으며 무료입니다. 사설 네트워크에서는 다음 이점을 제공합니다.
  * 장애 복구를 위해 다른 데이터 센터에 디바이스 환경 복제
  * 데이터베이스 서버에 대한 프론트 엔드 시스템 접근성
  * 시스템에 대한 안전한 액세스 및 관리

사용자가 사설 네트워크에 액세스할 수 있으려면 고객 포털에서 VPN 액세스를 편집하십시오.
  1. 메뉴 표시줄에서 **계정** > **VPN 액세스**를 선택하십시오.  
  2. VPN 액세스 열에서 링크를 클릭하십시오.
  3. **VPN 유형** 메뉴에서 옵션을 선택하고 **저장**을 클릭하십시오.  

IBM ID 인증을 사용하는 계정의 사용자인 경우에는 VPN 액세스를 위한 SoftLayer VPN 사용자 이름이 사용됩니다. VPN 사용자 이름은 사용자 프로파일에 정의되어 있고 IBM ID 이메일 주소 및 계정 ID로 기본 설정되는 사용자 이름과는 다릅니다.
{: tip}

VPN 연결 사용에 대한 자세한 정보는 [VPN 정보](/docs/infrastructure/iaas-vpn/about-vpn.html)를 참조하십시오.

## 4단계. 알림 구독
{: #get-notified}

발생할 수 있는 시스템 문제점 및 계획된 유지보수 이벤트에 대한 알림을 받으려면 이벤트 관리 시스템을 통해 알림을 구독할 수 있습니다. 기본적으로 계정을 작성하거나 계정에 추가할 때 알림 구독이 해제됩니다.

고객 포털의 이벤트 관리 시스템에 액세스하여 구독할 알림을 지정하십시오.
  1. 메뉴 표시줄에서 **계정** > **관리** > **구독**을 클릭하십시오.
  2. 목록에서 특정 구독을 클릭하십시오.
  3. 구독된 열의 선택란에서 **예**를 선택하십시오.
  4. **모든 구독 보기**를 클릭하여 사용 가능한 구독의 목록으로 돌아가서 필요한 경우 다른 유형을 구독하십시오.

## 다음 단계
{: #next-steps}

계정이 설정된 후 [{{site.data.keyword.Bluemix_notm}} 카탈로그 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://console.bluemix.net/catalog/?category=infrastructure){:new_window}로 이동하여 디바이스 주문을 시작하십시오.
