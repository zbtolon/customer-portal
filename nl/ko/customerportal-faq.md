---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-16"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# FAQ
{: #bicpfaq}

## 고객 포털에 대한 내 신임 정보를 검색하는 방법은 무엇입니까?
{: #bicp_retcreds}

인증을 위해 IBM ID를 사용하는 경우 처음 주문하거나 사용자로 계정에 추가될 때 IBM ID를 시작할 수 있는 링크가 포함된 이메일이 발송됩니다. 사용자 이름 또는 비밀번호를 잃어버렸거나 기억이 나지 않는 경우 [IBM ID 프로파일 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window}로 이동한 후 로그인 프로세스가 설명된 지시사항을 수행하여 비밀번호를 재설정하거나 복구하십시오. 특정 정보를 입력하도록 프롬프트가 표시되며, 보안 질문에 대한 답변 제공이 포함될 수 있습니다.

인증을 위해 IBM ID를 사용하지 않는 경우 처음 주문하거나 사용자로 [고객 포털 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 계정에 추가될 때 고객 포털을 시작할 수 있는 사용자 이름 및 초기 비밀번호가 포함된 이메일이 발송됩니다. 처음 로그인한 후에 사용자 프로파일을 편집하여 비밀번호를 변경해야 합니다. 

로그인한 후 비밀번호를 잊어버린 경우 고객 포털의 로그인 화면에서 사용 가능한 **비밀번호 찾기** 기능을 사용하십시오. 사용자 프로파일을 설정할 때 지정한 보안 질문 세트를 포함하여 특정 정보를 입력하도록 프롬프트가 표시됩니다.

사용자 이름을 잊어버린 경우 사용자 이름을 검색할 수 있는 계정 관리자 또는 마스터 관리자에게 문의하십시오. 계정의 마스터 사용자 또는 관리자인 경우에는 지원 센터에 문의하여 추가 지원을 받으십시오.

## IBM ID의 개념
{: #bicp_whatisibmid}

새 계정에는 인증을 위해 IBM ID가 필요합니다. 기존 계정은 마이그레이션 도구를 실행하여 IBM ID로 전환할 때까지 인증을 위해 SoftLayer 사용자 이름 및 비밀번호를 계속 사용합니다. SoftLayer 계정에는 동일한 계정 내에 더 많은 사용자를 추가할 수 있는 권한을 보유한 마스터 사용자가 있습니다. 자세한 정보는 [고객 포털에서 SoftLayer 계정이 관리되는 방법](/docs/customer-portal/cphowacctsman.html)을 참조하십시오.

## 기존 SoftLayer 계정을 연결하는 방법은 무엇입니까?
{: #bicp_linkbmxacct}

SoftLayer 계정의 마스터 사용자인 경우 고객 포털에 로그인한 후 헤더에서 **계정 연결**을 클릭하십시오. 자세한 정보는 [IBM ID 사용자 계정 연결](/docs/account/softlayerlink.html)을 참조하십시오.

## 기존 {{site.data.keyword.Bluemix_notm}} 사용자만 계정에 연결할 수 있습니까?
{: #bicp_bmxusertolink}

아니오. 새 {{site.data.keyword.Bluemix_notm}} 계정을 작성하거나 기존 {{site.data.keyword.Bluemix_notm}} 라이트 또는 종량과금제 계정을 연결할 수 있습니다.

## 이중 인증은 어떻게 작동됩니까?
{: #bicp_2fa}

계정 레벨에서는 이중 인증(2FA) 구성에 영향이 없습니다. 2FA는 IBM ID별로 수행되지 않고 계정별로 수행됩니다. IBM ID가 여러 계정과 연관되어 있고, 계정 간에 전환할 때는 2FA가 필요한 다른 계정으로 전환할 때마다 ID를 확인해야 합니다. 이는 이전 계정과 새 계정이 모두 같은 2FA 메커니즘으로 구성된 경우에도 해당됩니다.

2FA를 사용한 IBM ID의 자세한 정보는 [연결된 계정에서 이중 인증 사용](/docs/account/softlayerlink.html)을 참조하십시오.

## 누가 계정을 연결할 수 있습니까?
{: #bicp_wholinkaccts}

{{site.data.keyword.BluSoftlayer_notm}} 인프라 마스터 사용자만 SoftLayer와 {{site.data.keyword.Bluemix_notm}} 계정을 연결할 수 있습니다. 마스터 사용자의 이메일도 연결되어 있는 {{site.data.keyword.Bluemix_notm}} 계정의 기본 소유자와 연관되어야 합니다.

## 각 콘솔에 로그인하려면 무엇을 사용해야 합니까?
{: #bicp_logineachport}

계정 청구가 연결되어 있고 SoftLayer와 {{site.data.keyword.Bluemix_notm}} 계정 간에 쉽게 이동할 수 있으나 계정 ID는 계속 분리되어 있습니다.

* 계정에서 인증을 위해 IBM ID를 사용하지 않는 경우 계속해서 SoftLayer 제품 및 서비스에 SoftLayer ID를 사용하고 {{site.data.keyword.Bluemix_notm}} 제품 및 서비스에 IBM ID를 사용하십시오.

* 계정에서 인증을 위해 IBM ID를 사용하는 경우 IBM ID를 사용하여 SoftLayer 및 {{site.data.keyword.Bluemix_notm}} 계정 모두에 액세스하십시오.

## 내 SoftLayer 사용자 이름을 사용하여 로그인하려고 하면 오류가 발생하는 이유는 무엇입니까?
{: #bicp_SLloginerror}

IBM ID로 전환한 후 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사용자 이름으로 고객 포털에 로그인하는 경우 "Invalid login credentials provided" 오류가 표시됩니다. IBM ID로 전환한 후에는 더 이상 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사용자 이름으로 고객 포털에 로그인할 수 없습니다. 계정 로그인 대화 상자에서 **IBM ID로 로그인**을 클릭해야 합니다.

## 내 IBM ID를 사용하여 로그인하려고 하면 오류가 발생하는 이유는 무엇입니까?
{: #bicp_IBMidloginerror}

IBM ID로 로그인할 때 "We didn't recognize this IBMid or email" 오류가 표시됩니다. 완전한 이메일 주소를 입력했는지 확인하십시오. 또한 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사용자 이름을 사용하지 않았는지 확인하십시오.

## {{site.data.keyword.BluSoftlayer_notm}} 인프라 팀 구성원이 연결된 내 계정에 액세스할 수 있습니까?
{: #bicp_linkgiveteamaccess}

팀을 {{site.data.keyword.Bluemix_notm}}에 초대해야 합니다. {{site.data.keyword.Bluemix_notm}} 콘솔에서 **관리** > **계정** > **사용자**를 클릭하십시오. 리소스 그룹을 선택한 다음 {{site.data.keyword.BluSoftlayer_notm}} 인프라 팀 구성원을 추가할 수 있습니다. 고객 포털에 로그인해야 초대장을 보낼 수 있습니다. {{site.data.keyword.Bluemix_notm}}는 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사용자의 목록을 가져온 후 {{site.data.keyword.Bluemix_notm}} 계정에 초대할 사용자를 선택할 수 있습니다.

## IBM ID로 전환을 완료하기 위한 내 이메일은 어디에 있습니까?
{: #bicp_ibmidswitchemail}

IBM ID로 전환하기 위해 마법사를 따랐으나 이메일을 받지 못한 경우 등록 코드가 포함된 이메일이 발송되는 데 몇 분에서 몇 시간까지 소요될 수 있습니다. 고객 포털에서 **사용자 프로파일 편집** 페이지로 돌아간 후 **이메일 재발송**을 클릭하여 이메일 발송을 다시 시도할 수 있습니다.

## 내 계정에 대한 전체 루트 액세스가 있습니까?
{: #bicp_fullrootaccaccess}

마스터 사용자와 관리자 권한이 있는 사용자는 고객 포털 및 API의 계정에 대한 전체 루트 액세스 권한이 있습니다. 관리자 권한이 없는 사용자는 관리자 역할이 있는 사용자가 제어하는 접근성을 갖고 있습니다. 고객 포털에서 관리자가 [사용자 프로파일을 편집](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile)하여 이러한 권한을 업데이트할 수 있습니다. 관리자 권한이 없는 경우 고객 포털에서 맨 위 패널에 있는 사용자 이름을 클릭하여 사용자 프로파일을 편집할 수 있습니다.

## {{site.data.keyword.Bluemix_notm}} 구독 계정을 연결할 수 있습니까?
{: #bicp_linkbmxsubacct}

{{site.data.keyword.Bluemix_notm}}의 연결된 모든 계정은 라이트이거나 종량과금제 계정이어야 합니다. 

## 내 계정은 어떻게 연결 해제합니까?
{: #bicp_unlinkacct}

계정이 연결된 후에는 연결 해제할 수 없습니다.


## 내 회사 프로파일은 무엇이며, 어디서 찾을 수 있습니까?
{: #bicp_whatfindcompprof}

회사 프로파일은 계정이 작성된 당시에 제출된 정보이고 회사의 기본 연락처, 회사 이름, 주소 및 전화번호가 포함됩니다. 이 정보는 다양한 용도로 사용되며 항상 최신 상태로 유지되어야 합니다. 계정의 회사 프로파일을 보거나 변경을 요청하려면 [회사 프로파일 업데이트](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch)를 참조하십시오.

## 내 디바이스 및 소프트웨어 비밀번호를 어디서 찾을 수 있습니까?
{: #bicp_devswpw}

디바이스 및 소프트웨어 비밀번호는 고객 포털의 두 위치에 저장되어 있습니다. {{site.data.keyword.baremetal_short}} 및 {{site.data.keyword.virtualmachinesshort}}의
루트 또는 관리 사용자 이름과 비밀번호를 포함하여 디바이스 신임 정보를 검색하려면 [스냅샷 보기에서 디바이스와 상호작용](/docs/vsi/vsi_interact_device_snapshot_view.html)을 참조하십시오. 고객 포털을 사용하여 수동으로 추적된 소프트웨어 신임 정보를 빠르게 보고 검색하려면 [디바이스 액세스 관리](/docs/vsi/vsi_device_access.html)를 참조하십시오.

## 내 웹 데이터의 동기화를 유지하는 방법은 무엇입니까?
{: #bicp_webdatasync}

실제 서버 간에 데이터 일관성을 유지할 책임이 있지만, {{site.data.keyword.BluSoftlayer_full}}는 사용 비용 발생 없이 동기화하는 데 사용할 수 있는 사설 네트워크를 제공합니다.

## 이벤트 관리 시스템은 무엇입니까?
{: #bicp_whatisems}

이벤트 관리 시스템은 {{site.data.keyword.BluSoftlayer_full}}가 계획되지 않은 인프라 문제 및 다음 계획된 유지보수 이벤트에 대해 사용자와 정보를 공유하는 방식을 최적화하는 도구 세트입니다. 이는 발생한 이벤트의 유형을 공유하기 위해 이 인시던트와 관련되어 있는 대상으로 지정된 구독 기반 이메일 경보를 활용합니다. 이벤트의 전체 영향 및 진행 중인 계획되지 않은 인시던트(UIP)의 현재 상태에 대한 추가 세부사항을 포함하여 구독한 사용자를 제공합니다.

## 디바이스를 취소할 수 있습니까?
{: #bicp_candev}

고객 포털을 통해 언제든 디바이스를 취소할 수 있습니다. 취소 요청 완료에 대한 자세한 정보는 [디바이스 취소](/docs/vsi/vsi_managing.html)를 참조하십시오.
