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


# 入門指導教學
{: #getting-started}

在本指導教學中，我們將逐步解說使用 SoftLayer 帳戶開始進行以開始訂購及管理基礎架構資源的處理程序。
{:shortdesc}

## 開始之前
{: #prereqs}

您需要 [{{site.data.keyword.Bluemix}} 帳戶 ![外部鏈結圖示](../icons/launch-glyph.svg "外部鏈結圖示")](https://console.bluemix.net/){:new_window}。使用 IBM ID 認證來登入客戶入口網站。大部分的新使用者會使用 [IBM ID](/docs/account/softlayerlink.html#switchtoIBMid) 進行鑑別。

如果您在登入帳戶時未使用 IBM ID 進行鑑別，則請使用您的唯一 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構認證來登入客戶入口網站。
{: tip}

## 步驟 1. 設定帳戶
{: #account-setup}

設定帳戶包括驗證帳戶聯絡資訊及計費詳細資料：
 * 若要驗證公司聯絡詳細資料，請移至**帳戶** > **管理** > **公司聯絡人**。您帳戶的公司聯絡資訊會用來通知您有關帳戶的任何問題或變更。
 * 若要驗證公司設定檔詳細資料，請移至**帳戶** > **管理** > **公司設定檔**。公司設定檔資訊包含關於主要帳戶持有者的相關詳細資料。
 * 若要驗證您的計費詳細資料，請移至**帳戶** > **計費** > **付款方法**。每月付款方法是使用信用卡，將會週期性地用來支付與帳戶相關聯的款項。

## 步驟 2. 新增使用者及指派許可權
{: #users-permissions}

若要將使用者新增至您的帳戶，並設定起始許可權，請移至**帳戶** > **使用者**。
 * 若要邀請使用者根據您指派的特定許可權使用您帳戶中的平台及基礎架構資源，請按一下**邀請使用者**。接著會將您導向至 {{site.data.keyword.Bluemix_notm}} Identity and Access Management (Tivoli Information Archive Manager) 使用者介面，來邀請使用者以及指派存取權。如需相關資訊，請參閱[邀請使用者及指派存取權](/docs/iam/iamuserinv.html)。
 * 若要新增僅具有 VPN 存取權的使用者，請按一下**新增僅限 VPN 使用者**。請輸入個人資訊、設定入口網站許可權，以及設定使用者的裝置存取權。

當您在起始邀請中設定基礎架構許可權時，請選擇三個許可權集中的其中一個：「僅限檢視」、「基本使用者」、「超級使用者」。使用者接受邀請之後，您就可以藉由編輯其入口網站許可權來自訂其存取。如需相關資訊，請參閱[基礎架構許可權](/docs/iam/infrastructureaccess.html)。
{: tip}

## 步驟 3. 啟用 {{site.data.keyword.Bluemix_notm}} 基礎架構專用網路的存取
{: #enable-private-network}

{{site.data.keyword.Bluemix_notm}} 基礎架構專用網路免費提供給使用者及裝置使用。專用網路上的所有頻寬都不限流量而且免費贈送。專用網路提供下列好處：
  * 將裝置環境抄寫至其他資料中心以進行失效接手
  * 資料庫伺服器的前端系統存取性
  * 系統的安全存取及管理

若要讓使用者存取專用網路，請在客戶入口網站中編輯 VPN 存取權：
  1. 從功能表列中，選取**帳戶** > **VPN 存取權**。  
  2. 按一下「VPN 存取權」直欄中的鏈結。
  3. 從 **VPN 類型**功能表中選取選項，然後按一下**儲存**。  

針對帳戶中使用 IBM ID 鑑別的使用者，會使用 SoftLayer VPN 使用者名稱進行 VPN 存取。VPN 使用者名稱定義於使用者設定檔中，且與預設為 IBM ID 電子郵件位址及帳戶 ID 的使用者名稱不同。
{: tip}

如需使用 VPN 連線的相關資訊，請參閱[關於 VPN](/docs/infrastructure/iaas-vpn/about-vpn.html)。

## 步驟 4. 訂閱通知
{: #get-notified}

若要收到可能發生之系統問題及計劃性維護事件的通知，您可以透過「事件管理系統」來訂閱通知。當您建立帳戶或已將您新增至帳戶時，依預設，會取消訂閱通知。

在客戶入口網站中存取「事件管理系統」，以指定您要訂閱的通知：
  1. 從功能表列中，選取**帳戶** > **管理** > **訂閱**。
  2. 從清單中按一下特定訂閱。
  3. 在「已訂閱」直欄中，選取**是**。
  4. 按一下**檢視所有訂閱**以回到可用的訂閱清單，並訂閱其他類型（必要的話）。

## 後續步驟
{: #next-steps}

設定帳戶之後，請移至 [{{site.data.keyword.Bluemix_notm}} 型錄 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://console.bluemix.net/catalog/?category=infrastructure){:new_window}，並開始訂購裝置。
