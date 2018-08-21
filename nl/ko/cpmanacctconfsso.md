---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-13"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 싱글 사인온 구성
{: #customerportal_confssoserv}

계정의 마스터 사용자이거나 계정에 대한 관리 액세스 권한이 있는 경우 싱글 사인온을 구성할 수 있습니다. {{site.data.keyword.BluSoftlayer_full}} 인프라에 대한 싱글 사인온 구성은 2단계 프로세스입니다. 먼저, ID 제공자를 선택하고 설정하십시오. 그런 다음, {{site.data.keyword.BluSoftlayer_notm}} 인프라를 설정하여 ID 제공자로부터 인증 유형을 수신하십시오.
{:shortdesc}

## ID 제공자 선택 및 설정
{: #cp_setupidprov}

ID 제공자가 없는 경우 먼저 ID 제공자를 선택하고 설정하십시오. {{site.data.keyword.BluSoftlayer_notm}}와 함께 다음 ID 제공자를 사용할 수 있습니다.
* Ping Identity&reg;
* OneLogin&trade;
* IBM&reg; Cloud Security Enforcer
* IBM Cloud Identity Services
자세한 정보는 {{site.data.keyword.BluSoftlayer_notm}} 인프라 영업 담당자에게 문의하십시오.

ID 제공업체가 아직 설정되지 않은 경우 ID 제공자 지원에 특정 단계에 대해 문의할 수 있습니다. 또는 다음 상위 레벨 단계를 사용하여 ID 제공자를 구성할 수도 있습니다.
1. 실행 파일을 다운로드하고 설치하여 ID 제공자 환경을 준비하십시오.
2. ID 제공자를 구성하여 {{site.data.keyword.BluSoftlayer_notm}} 인증에 대해 작업하십시오.

## SSO용 {{site.data.keyword.BluSoftlayer_notm}} 인프라 설정
{: #cp_setupsso}

{{site.data.keyword.BluSoftlayer_notm}}와 함께 사용하려면 ID 제공자에서 SAML&trade;(Security Assertion Markup Language&trade;) 2.0 메타데이터 정보의 다음 필수 필드를 추출해야 합니다.
<dl>
<dt>엔티티 ID</dt>
<dd>ID 제공자의 엔티티 ID</dd>
<dt>싱글 사인온 URL</dt>
<dd>SSO용 ID 제공자의 엔드포인트</dd>
<dt>인증서</dt>
<dd>요청을 서명하는 데 사용된 ID 제공자의 인증서</dd>
<dt>인증서 지문</dt>
<dd>인증서의 지문입니다. 전체 인증서 대신 이 필드를 사용할 수 있습니다(선택사항).</dd>
</dl>

ID 제공자로부터 인증 유형을 수신하기 위해 {{site.data.keyword.BluSoftlayer_notm}} 인프라를 설정하려면 다음 단계를 수행하십시오.
1. ID 제공자에 로그인하고, 아직 로그인하지 않은 경우 **SAML 구성** 페이지를 찾으십시오. 다음 정보를 참조하십시오.
  * 엔티티 ID
  * 싱글 사인온 URL
  * 인증서(인증서 요구사항은 ID 제공자에 따라 달라짐)
2. SoftLayer 계정을 작성하는 데 사용한 마스터 사용자 이름 및 비밀번호를 사용하여 마스터 사용자로 {{site.data.keyword.BluSoftlayer_notm}} 인프라에 로그인하십시오.
3. **계정** > **관리** > **SAML 인증**을 클릭하십시오.
4. **ID 제공자** 메타데이터를 입력하십시오.
5. **저장**을 클릭하십시오.
6. **계정** > **관리** > **SAML 인증**을 클릭하십시오.
7. **XML 구성 다운로드**를 클릭하여 서비스 제공자 메타데이터를 다운로드하거나 정보를 작성하십시오.
8. **서비스 제공자** 메타데이터를 사용하여 ID 제공자의 지시사항에 따라 ID 제공자를 구성하십시오.  

연합 ID를 사용하여 {{site.data.keyword.BluSoftlayer_notm}} 인프라에 로그인할 수 있습니다. 연합 ID에 대한 자세한 정보는 [{{site.data.keyword.Bluemix_notm}} 등록](/docs/account/adminpublic.html) 및 [IBMid Enterprise Federation Adoption Guide ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}를 참조하십시오.
