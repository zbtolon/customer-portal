---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-19"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# SoftLayer API
{: #customerportal_api}

在開發環境中使用直接 API 呼叫（而非使用客戶入口網站），即可使用 API 與帳戶、產品及服務互動。
{:shortdesc}

API 的目標是提供您可以在 API 中完成任何客戶入口網站作業的環境。API 環境是透過頻繁地新增及更新進行維護，確保您有最佳選項可供使用。這包括可以使用各種語言及選項來設計程式，以使用 SOAP、XML-RPC 及 REST 型 API。與在客戶入口網站中運作類似，如果您主要在 API 中進行帳戶互動，則也需要可行的支援來源。

## 如何存取 API？
{: #cp_getapikey}

您可以藉由使用者特有的API 金鑰來存取 API。API 金鑰是唯一的英數 ID，可讓您安全地存取 API。您的 API 金鑰專門鏈結到您的使用者 ID，且此 API 金鑰能在 API 中提供與您在「客戶入口網站」中 具備 的相同許可權。您產生一次 API 金鑰，接下來就可以擷取它並繼續使用。請使用下列步驟，以產生您的 API 金鑰：

1. 使用唯一的認證來存取客戶入口網站。
2. 從導覽列中，選取**帳戶** > **使用者**。
3. 在具有使用者認證之列的 **API 金鑰**直欄下，按一下**產生**鏈結。

產生 API 金鑰之後，**產生**鏈結會變更為**檢視**鏈結，您可以隨時用來存取 API 金鑰。

## 哪裡可以進一步瞭解 API？
{: #cp_apimoreinfo}

使用 API 與帳戶、產品及服務互動時，[SoftLayer Development Network (SLDN) ![外部鏈結圖示](../icons/launch-glyph.svg)](http://sldn.softlayer.com/){:new_window} 專用於支援您。[SLDN ![外部鏈結圖示](../icons/launch-glyph.svg)](http://sldn.softlayer.com/){:new_window} 包含 SoftLayer API、所支援程式設計語言、可用 API 呼叫等等的相關文件。SLDN 是資源，用於提供各種 API 特性、完整 API 呼叫清單及各種部落格文章的資訊，讓您知道如何最恰當地使用 API。


如果您有任何 API 問題，可以將它們張貼至客戶討論區，或透過文章直接提出意見。
