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

계정을 설정할 때 기존 IBM ID 이메일 주소를 사용하여 하나의 IBM ID를 여러 SoftLayer 계정과 연관시킬 수 있습니다. 각 계정에 대한 한 명의 {{site.data.keyword.BluSoftlayer_notm}} 인프라 사용자만 단일 IBM ID로 맵핑될 수 있습니다. IBM ID는 각 SoftLayer 계정 내에서 고유해야 합니다. 그러나 계정에 대한 액세스 권한이 있는 한 명의 사용자가 여러 SoftLayer 계정에 액세스할 수 있는 하나의 IBM ID를 사용할 수 있습니다.

하나의 IBM ID가 계정 A 및 B의 마스터 사용자와 계정 C 및 D의 추가 사용자에 맵핑될 수 있습니다. 해당 IBM ID에 맵핑된 계정 중 하나가 기본 계정이 됩니다. 일반적으로 기본 계정은 IBM ID로 처음 맵핑되는 계정입니다. 그러나 고객 포털의 계정 전환 기능을 사용하여 기본 계정을 전환할 수 있습니다.

![여러 SoftLayer 계정을 하나의 IBM ID로 맵핑](images/ibmid-image.png)

이중 인증(2FA)이 사용으로 설정된 여러 계정에 대한 IBM ID 액세스 권한이 있는 사용자의 경우에는 2FA 확인 코드가 필요합니다. 이 확인 코드는 계정 로그인 중에, 그리고 기본 계정에서 전환할 때 계정마다 필요합니다.
