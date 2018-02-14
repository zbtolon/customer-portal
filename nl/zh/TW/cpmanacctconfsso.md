---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 配置單一登入
{: #customerportal_confssoserv}

如果您是帳戶的主要使用者，或具有其管理存取權，則可以配置單一登入。配置 {{site.data.keyword.BluSoftlayer_full}} 基礎架構的單一登入是兩步驟的處理程序。首先，請選取並設定身分提供者。然後，設定 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構接收來自身分提供者的鑑別要求。
{:shortdesc}

## 選取並設定身分提供者
{: #cp_setupidprov}

如果您還沒有身分提供者，請先選取一個身分提供者，並進行設定。您可以搭配使用下列身分提供者與 {{site.data.keyword.BluSoftlayer_notm}}：
* Ping Identity&reg;、
* OneLogin&trade;、
* IBM&reg; Cloud Security Enforcer、
* IBM Cloud Identity Services。
如需相關資訊，請聯絡 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構業務代表。

如果您尚未設定身分提供者，可以聯絡特定步驟的身分提供者支援，或使用下列高階步驟來配置身分提供者：
1. 下載並安裝身分提供者執行檔，以準備身分提供者環境。
2. 配置身分提供者，以使用 {{site.data.keyword.BluSoftlayer_notm}} 鑑別。

## 設定 SSO 的 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構
{: #cp_setupsso}

您必須從身分提供者擷取 Security Assertion Markup Language&trade; (SAML&trade;) 2.0 Meta 資料資訊的下列必要欄位，以與 {{site.data.keyword.BluSoftlayer_notm}} 搭配使用。
<dl>
<dt>實體 ID</dt>
<dd>身分提供者的實體 ID。</dd>
<dt>單一登入 URL</dt>
<dd>SSO 之身分提供者的端點。</dd>
<dt>憑證</dt>
<dd>用來簽署要求的身分提供者憑證。</dd>
</dl>

下列是選用欄位：
<dl>
<dt>憑證指紋</dt>
<dd>憑證的指紋。您可以使用此欄位，而非整個憑證。</dd>
</dl>

請使用下列步驟，以設定 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構接收來自身分提供者的鑑別要求：
1. 登入身分提供者（如果尚未登入），並找出 **SAML 配置**頁面。請注意下列資訊：
  * 實體 ID
  * 單一登入 URL
  * 憑證（這會根據身分提供者而不同。）
2. 使用您用來建立 SoftLayer 帳戶的主要使用者名稱及密碼，以主要使用者身分登入 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構。
3. 按一下**帳戶** > **管理** > **SAML 鑑別**。
4. 輸入**身分提供者** meta 資料。
5. 按一下**儲存**。
6. 按一下**帳戶** > **管理** > **SAML 鑑別**。
7. 按一下**下載 XML 配置**，以下載服務提供者 meta 資料，或趕快記下資訊。
8. 使用**服務提供者** meta 資料，以根據身分提供者指示來配置身分提供者。  

您現在應該可以使用聯合 ID 來登入 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構。
