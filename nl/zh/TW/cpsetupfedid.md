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

# 設定識別身分同盟
{: #cp_setupidfed}

您可以設定識別身分同盟，讓服務提供者（例如 {{site.data.keyword.BluSoftlayer_full}} 基礎架構管理系統 (IMS)）使用授信身分系統所產生的安全記號來進行鑑別及授權。
{:shortdesc}

您可以使用下列其中一種方式，在 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構 SSO 中設定識別身分同盟：
* 在身分提供者及 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構中建立使用者
* 在身分提供者中建立使用者

針對服務提供者，角色定義在鑑別使用者之後授權使用者在其系統中執行的作業（透過許可權）。例如，可能只允許*使用者* 角色檢視不同的畫面，而無法進行更新或新增。

可以將多位使用者指派給單一角色。而且，如果角色存在於身分提供者中，但不存在於 {{site.data.keyword.BluSoftlayer}} 基礎架構中，則使用者仍然可以登入 {{site.data.keyword.BluSoftlayer}} 基礎架構，但使用者沒有任何指派給角色的許可權。
{: tip}


## 在身分提供者及 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構中建立使用者
{: #cp_scenario1both}

在此模型中，會發生下列事項：
* 在身分提供者及 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構中，建立使用者。
* 使用 {{site.data.keyword.BluSoftlayer}} 基礎架構客戶入口網站或 API，在 {{site.data.keyword.BluSoftlayer}} 基礎架構 IMS 中指派使用者許可權。
* 使用者會鑑別身分提供者，並聯合其認證。
* {{site.data.keyword.BluSoftlayer}} 基礎架構會使用認證，而且存取控制是根據在 {{site.data.keyword.BluSoftlayer}} 基礎架構 IMS 中針對使用者所定義的許可權。

使用隨機密碼，先在 {{site.data.keyword.BluSoftlayer}} 基礎架構中建立需要存取 {{site.data.keyword.BluSoftlayer}} 基礎架構之使用者的帳戶。必須先在 {{site.data.keyword.BluSoftlayer}} 基礎架構中配置所有許可權，使用者才能透過身分提供者來使用 SSO。目前是根據個別使用者來設定許可權。

### 設定使用者
請使用下列步驟，以設定使用者：

1. [在 {{site.data.keyword.BluSoftlayer}} 基礎架構中建立使用者](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct)。
2. 在 {{site.data.keyword.BluSoftlayer}} 基礎架構中指派許可權。
3. 在身分提供者中建立使用者。

個別使用者設定檔內的**電子郵件**或**使用者名稱**欄位是用於 Security Assertion Markup Language&trade; (SAML&trade;) 2.0 記號，而此記號可在身分提供者與 {{site.data.keyword.BluSoftlayer}} 基礎架構之間對映使用者。

### 登入鑑別範例流程
以下範例流程說明在身分提供者及 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構中建立使用者時使用者登入鑑別的運作方式：
1. 使用者從瀏覽器階段作業中存取身分提供者 URL。
2. 身分提供者會鑑別使用者，例如，透過其 LDAP。
3. 身分提供者會傳回 SAML 2.0 回應。
4. 身分提供者會將 SAML 2.0 回應傳送至服務提供者（在此情況下是 {{site.data.keyword.BluSoftlayer}} 基礎架構），以鑑別使用者 ID。
5. {{site.data.keyword.BluSoftlayer}} 基礎架構會驗證 SAML 2.0 回應。
6. 使用者會根據身分提供者與 {{site.data.keyword.BluSoftlayer}} 基礎架構之間的授信設定來登入 {{site.data.keyword.BluSoftlayer}} 基礎架構客戶入口網站。


## 在身分提供者中建立使用者
{: #cp_scenario2idp}

在此模型中，會發生下列事項：
* 在身分提供者中建立角色，並將其指派給使用者。
* 使用 {{site.data.keyword.BluSoftlayer}} 基礎架構 API，在 {{site.data.keyword.BluSoftlayer}} 基礎架構 IMS 中設定角色及許可權指派。
* 使用者會鑑別身分提供者，並聯合其認證及角色屬性。
* {{site.data.keyword.BluSoftlayer}} 基礎架構會利用使用者認證及角色屬性。如果使用者的身分提供者已指派角色符合 {{site.data.keyword.BluSoftlayer}} 基礎架構中的角色，則使用者會在登入 {{site.data.keyword.BluSoftlayer}} 基礎架構時獲指派該角色的許可權。
* 會將身分提供者中所建立的使用者視為聯合，因為他們及其角色是透過 SAML 2.0 進行鑑別。

### 設定使用者的角色
請使用下列步驟，以設定使用者的角色：

1. 透過 {{site.data.keyword.BluSoftlayer}} 基礎架構 API 設定角色。
2. 在身分提供者中設定角色。
3. 確定 {{site.data.keyword.BluSoftlayer}} 基礎架構及身分提供者中所定義的角色同名。

### 設定使用者
{: #setupuser}

請使用下列步驟，以設定使用者：

1. 在身分提供者中設定使用者。
2. 在身分提供者中，將角色指派給使用者。

在此情境下，您不需要在 {{site.data.keyword.BluSoftlayer}} 基礎架構中手動建立使用者。

### 使用者登入鑑別範例流程
以下範例流程說明在身分提供者中建立使用者時使用者登入鑑別的運作方式：
1. 使用者從瀏覽器階段作業中存取身分提供者 URL。
2. 身分提供者會鑑別使用者，例如，透過其 LDAP。
3. 身分提供者會傳回 SAML 2.0 回應。
4. 身分提供者會將 SAML 2.0 回應傳送至服務提供者（在此情況下是 {{site.data.keyword.BluSoftlayer}} 基礎架構），以鑑別使用者角色。
5. {{site.data.keyword.BluSoftlayer}} 基礎架構會驗證 SAML 2.0 回應。
6. {{site.data.keyword.BluSoftlayer}} 基礎架構將使用者重新導向至客戶入口網站。
7. 使用者已登入 {{site.data.keyword.BluSoftlayer}} 基礎架構客戶入口網站。

請檢閱身分提供者有關設定新角色以及如何建立其與 {{site.data.keyword.BluSoftlayer}} 基礎架構之關聯的程序。
