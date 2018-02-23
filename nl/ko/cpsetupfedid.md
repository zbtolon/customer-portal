---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# ID 연합 설정
{: #cp_setupidfed}

{{site.data.keyword.BluSoftlayer_full}} Infrastructure Management System(IMS)과 같은 서비스 제공자를 사용할 수 있도록 ID 연합을 설정하여
인증 및 권한 부여를 위해 신뢰할 수 있는 ID 시스템에서 생성된 보안 토큰을 이용하십시오.
{:shortdesc}

다음 방법 중 하나를 사용하여 {{site.data.keyword.BluSoftlayer_notm}} 인프라 SSO에서 ID 연합을 설정할 수 있습니다.
* ID 제공자 및 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 사용자 작성
* ID 제공자에서 사용자 작성

역할은 서비스 제공자를 위해 사용자가 인증된 후 시스템에서 사용자가 권한이 부여되어 수행하는(권한을 통해) 작업을 정의합니다. 예를 들어, *User* 역할은 다른 화면만 보도록 허용될 수 있으나 업데이트하거나 추가할 수 없을 수 있습니다.

다중 사용자를 단일 역할에 지정할 수 없습니다. 또한 역할이 ID 제공자에 존재하지만 {{site.data.keyword.BluSoftlayer}} 인프라에 존재하지 않는 경우 사용자는 계속해서 {{site.data.keyword.BluSoftlayer}} 인프라에 로그인할 수 있으나 역할에 지정된 권한은 제공되지 않습니다.
{: tip}


## ID 제공자 및 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 사용자 작성
{: #cp_scenario1both}

이 모델에서 다음 사항이 발생합니다.
* 사용자는 ID 제공자 및 {{site.data.keyword.BluSoftlayer_notm}} 인프라 모두에서 작성됩니다 .
* 사용자 권한은 {{site.data.keyword.BluSoftlayer}} 인프라 고객 포털 또는 API를 사용하여 {{site.data.keyword.BluSoftlayer}} 인프라에 지정됩니다.
* 사용자는 ID 제공자로 인증하고 신임 정보를 연합합니다.
* {{site.data.keyword.BluSoftlayer}} 인프라는 신임 정보를 이용하고 액세스 제어는 {{site.data.keyword.BluSoftlayer}} 인프라 IMS에서 사용자에 대해 정의된 권한을 기반으로 합니다.

{{site.data.keyword.BluSoftlayer}} 인프라에 액세스하는 데 필요한 사용자의 계정은 먼저 랜덤 비밀번호를 포함하여
{{site.data.keyword.BluSoftlayer}} 인프라에 작성됩니다. 사용자가 ID 제공자를 통해 SSO를 사용하기 전에 모든 권한이 {{site.data.keyword.BluSoftlayer}} 인프라에 구성되어야 합니다. 현재 권한은 개별 사용자를 기반으로 설정됩니다.

### 사용자 설정
사용자를 설정하려면 다음 단계를 수행하십시오.

1. [{{site.data.keyword.BluSoftlayer}} 인프라에서 사용자를 작성하십시오.](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. {{site.data.keyword.BluSoftlayer}} 인프라에서 권한을 지정하십시오.
3. ID 제공자에서 사용자를 작성하십시오.

개별 사용자 프로파일 내 **이메일** 또는 **사용자 이름** 필드는 Security Assertion Markup Language&trade;(SAML&trade;) 2.0 토큰에 사용되며,
이는 ID 제공자 및 {{site.data.keyword.BluSoftlayer}} 인프라 간의 사용자를 맵핑합니다.

### 로그인 인증에 대한 플로우 예제
다음은 ID 제공자 및 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 사용자를 작성할 때 사용자 로그인 인증이 작동하는 방식의 플로우 예제입니다.
1. 사용자는 브라우저 세션에서 ID 제공자 URL에 액세스합니다.
2. ID 제공자는 사용자를 인증합니다(예: LDAP을 통해).
3. ID 제공자는 SAML 2.0 응답을 리턴합니다.
4. {{site.data.keyword.BluSoftlayer}} 인프라의 경우, ID 제공자는 SAML 2.0 응답을 서비스 제공자에게 전송하여 사용자 ID를 인증합니다.
5. {{site.data.keyword.BluSoftlayer}} 인프라는 SAML 2.0 응답을 유효성 검증합니다.
6. 사용자는 ID 제공자 및 {{site.data.keyword.BluSoftlayer}} 인프라 간의 신뢰할 수 있는 설정을 기반으로 {{site.data.keyword.BluSoftlayer}} 인프라 고객 포털에 로그인됩니다.


## ID 제공자에서 사용자 작성
{: #cp_scenario2idp}

이 모델에서 다음 사항이 발생합니다.
* 역할은 ID 제공자에서 작성되고 사용자에게 지정됩니다.
* 역할 및 권한 지정은 {{site.data.keyword.BluSoftlayer}} 인프라 API를 사용하여 {{site.data.keyword.BluSoftlayer}} 인프라 IMS에서 설정됩니다.
* 사용자는 ID 제공자로 인증하고 신임 정보 및 역할 속성을 연합합니다.
* {{site.data.keyword.BluSoftlayer}} 인프라는 사용자 신임 정보 및 역할 속성을 이용합니다. 역할이 지정된 사용자의 ID 제공자가
{{site.data.keyword.BluSoftlayer}} 인프라의 역할과 일치하는 경우 사용자는 {{site.data.keyword.BluSoftlayer}} 인프라에 로그인할 때 해당 역할에 대한 권한을 부여받습니다.
* ID 제공자에서 작성된 사용자 및 해당 역할이 SAML 2.0을 통해 인증되었기 때문에 이 사용자는 연합된 것으로 간주됩니다.

### 사용자에 대한 역할 설정
사용자에 대한 역할을 설정하려면 다음 단계를 수행하십시오.

1. {{site.data.keyword.BluSoftlayer}} 인프라 API를 통해 역할을 설정하십시오.
2. ID 제공자에서 역할을 설정하십시오.
3. {{site.data.keyword.BluSoftlayer}} 인프라에서 정의된 역할과 ID 제공자의 이름이 동일한지 확인하십시오.

### 사용자 설정
{: #setupuser}

사용자를 설정하려면 다음 단계를 수행하십시오.

1. ID 제공자에서 사용자를 설정하십시오.
2. ID 제공자에서 역할을 사용자에게 지정하십시오.

이 시나리오에서는 사용자를 {{site.data.keyword.BluSoftlayer}} 인프라에서 수동으로 작성할 필요가 없습니다.

### 사용자 로그인 인증에 대한 플로우 예제
다음은 ID 제공자에서 사용자를 작성할 때 사용자 로그인 인증이 작동하는 방식의 플로우 예제입니다.
1. 사용자는 브라우저 세션에서 ID 제공자 URL에 액세스합니다.
2. ID 제공자는 사용자를 인증합니다(예: LDAP을 통해).
3. ID 제공자는 SAML 2.0 응답을 리턴합니다.
4. {{site.data.keyword.BluSoftlayer}} 인프라의 경우, ID 제공자는 SAML 2.0 응답을 서비스 제공자에게 전송하여 사용자 역할을 인증합니다.
5. {{site.data.keyword.BluSoftlayer}} 인프라는 SAML 2.0 응답을 유효성 검증합니다.
6. {{site.data.keyword.BluSoftlayer}} 인프라는 사용자 포털로 사용자를 경로 재지정합니다.
7. 사용자는 {{site.data.keyword.BluSoftlayer}} 인프라 고객 포털에 로그인됩니다.

새 역할 설정에 대한 ID 제공자의 프로시저와 새 역할을 {{site.data.keyword.BluSoftlayer}} 인프라와 연관시키는 방법을 검토하십시오.
