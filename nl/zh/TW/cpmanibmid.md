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

# 搭配使用 IBM ID 帳戶與 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構
{: #customerportal_ibmid}

{{site.data.keyword.BluSoftlayer_notm}} 基礎架構中的鑑別現在使用 IBM ID 來提供 {{site.data.keyword.Bluemix_notm}} 的單一登入。
{:shortdesc}

如果您有現有的 SoftLayer 帳戶，則可以切換至 IBM ID。移轉精靈可協助引導您完成這項切換。如需相關資訊，請參閱[切換至 IBM ID](/docs/account/softlayerlink.html#switching-to-ibmid)。

## 將多個 SoftLayer 帳戶對映至一個 IBM ID
{: #cp_mapmultclinfrto1ibmid}

設定帳戶時，您可以使用現有 IBM ID 電子郵件位址來建立一個 IBM ID 與多個 SoftLayer 帳戶的關聯。每一個帳戶只有一個 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用者可以對映至單一 IBM ID。在每一個 SoftLayer 帳戶內，IBM ID 都必須是唯一的。不過，一個可存取多個 SoftLayer 帳戶的使用者可以使用一個 IBM ID 來存取多個 SoftLayer 帳戶。

例如，IBM ID 可以對映至帳戶 A 及 B 中的主要使用者，以及帳戶 C 及 D 中的另一個使用者。對映至該 IBM ID 的其中一個帳戶就是預設帳戶。通常，預設帳戶是第一個對映至 IBM ID 的帳戶。不過，您可以在客戶入口網站中透過帳戶切換特性來切換哪個帳戶才是預設帳戶。

![多個 SoftLayer 帳戶對一個 IBM ID](images/ibmid-image.png)

針對使用 IBM ID 存取多個已啟用雙因子鑑別之帳戶的使用者，需要有雙因子鑑別驗證碼。在帳戶登入期間，以及當您切換預設帳戶時，每個帳戶都需要驗證碼。
