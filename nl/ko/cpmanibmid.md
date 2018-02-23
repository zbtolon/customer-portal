---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-10"

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:tip: .tip}
{:codeblock: .codeblock}
{:pre: .pre}
{:new_window: target="_blank"}

# {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 IBM ID 계정 사용
{: #customerportal_ibmid}

이제 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서의 인증은 {{site.data.keyword.Bluemix_notm}}에 대한 단일 로그인을 제공하는 IBM ID를 사용합니다.
{:shortdesc}

기존 SoftLayer 계정이 있는 경우 IBM ID로 전환할 수 있습니다. 마이그레이션 마법사가 이 전환을 통해 사용자를 안내할 수 있습니다. 자세한 정보는 [IBM ID로 전환](/docs/account/softlayerlink.html#switching-to-ibmid)을 참조하십시오.

## 여러 SoftLayer 계정을 하나의 IBM ID로 맵핑
{: #cp_mapmultclinfrto1ibmid}

주문을 설정할 때 기존 IBM ID 이메일 주소를 사용하여 하나의 IBM ID를 여러 SoftLayer 계정과 연관시킬 수 있습니다. 각 계정에 대한 한 명의 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사용자만 단일 IBM ID로 맵핑될 수 있습니다. IBM ID는 각 SoftLayer 계정 내에서 고유해야 합니다. 그러나 여러 SoftLayer 계정에 대한 액세스 권한이 있는 한 명의 사용자가 여러 SoftLayer 계정에 액세스할 수 있는 하나의 IBM ID를 사용할 수 있습니다.

예를 들어, IBM ID는 계정 A 및 B의 마스터 사용자 및 계정 C 및 계정 D의 추가 사용자로 맵핑할 수 있습니다. 해당 IBM ID로 맵핑되는 계정 중 하나가 기본 계정이 됩니다. 일반적으로 기본 계정은 IBM ID로 처음 맵핑되는 계정입니다. 그러나 고객 포털의 계정 전환 기능을 통해 계정(기본 계정)을 전환할 수 있습니다.

![여러 SoftLayer 계정을 하나의 IBM ID로 맵핑](images/ibmid-image.png)

이중 인증이 사용된 여러 계정에 대한 IBM ID 액세스 권한이 있는 사용자의 경우 계정 로그인 및 계정 전환 중에 적절한 이중 인증 확인 코드(계좌당)가 필요합니다.
