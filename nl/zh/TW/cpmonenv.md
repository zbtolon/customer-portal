---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 監視環境及系統事件
{: #customerportal_cpmonenvsysevent}

監視環境表示您隨時可以檢查裝置，而且您會在其中一個裝置關閉時自動收到通知。您也可以監視系統事件，讓系統流暢地執行。  
{: shortdesc}

## 監視環境
{: #cpmonenv}

最少要使用基本連線測試監視，但您可以使用最符合商業需求的方式來自訂監視選項。

### 隨時接收網路維護及非計劃性事件的通知
{: #cp_stayinfomaintevent}

有時候，排定及緊急網路維護是不可避免的。{{site.data.keyword.BluSoftlayer_full}} 基礎架構會維護許多通道，讓您可以收到所有排定及緊急維護事件的通知。此外，您還可以從「事件管理系統」中[訂閱電子郵件通知](/docs/customer-portal/cpsub2not.html)。此增補服務會自動將有關可能影響服務之非計劃性事件的電子郵件傳送給訂閱的使用者。

### 使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構行動
{: #cp_bmxinframobile}

使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構行動，和 iOS 或 Android 行動裝置，隨時隨地管理 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構裝置。{{site.data.keyword.BluSoftlayer_notm}} 基礎架構行動內的功能包括問題單支援、基本裝置控制及頻寬監視。

{{site.data.keyword.BluSoftlayer_notm}} 基礎架構行動應用程式能補充客戶入口網站的功能，因為您可以從任何地方使用連接網路的行動裝置來監視基礎架構的重要資訊。雖然應用程式演進快速且會定期新增功能，您仍可使用行動應用程式來執行如下作業：
  * 檢視、建立及更新支援問題單
  * 監視裝置狀態，包括頻寬及警示
  * 關閉及重新啟動裸機伺服器與虛擬伺服器
  * 檢視帳戶發票並進行一次性付款
  * 存取及檢查 Object Storage 中儲存的內容

可在數個熱門行動裝置平台上使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構行動應用程式，且可以在每一個平台的相關應用程式商店中免費取得。

## 監視伺服器
{: #customerportal_monservers}

設定監視來檢查伺服器的狀態，以瞭解何時需要擴充。您可以使用標準監視或 Nimsoft 監視服務。您可以透過在 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構客戶入口網站中使用慢速或服務連線測試，以連線測試及回應 (ping-and-respond) 方法進行標準（或基本）監視。您也可以使用客戶入口網站中的 Nimsoft（或進階）監視，或是在下列三層其中之一進行監視：基本、進階及超值。明確地說，如需裸機伺服器的相關資訊，請參閱[開始使用裸機伺服器](/docs/bare-metal/about.html)。

## 監視系統事件
{: #customerportal_monevent}

您可以檢視審核日誌及存取日誌，以監視系統事件。

### 檢視帳戶的審核日誌
{: #cp_viewacctauditlog}

每一個客戶入口網站帳戶都會隨附審核日誌，以追蹤客戶入口網站內每一位使用者的互動。例如，會追蹤下列互動：
  * 登入嘗試（成功及失敗）
  * 埠速度更新
  * 開關電源及重新啟動
  * {{site.data.keyword.BluSoftlayer_notm}} 基礎架構支援人員所做的互動。

請使用下列步驟，以檢視使用者帳戶的審核日誌。

1. 使用唯一的認證來存取[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 從導覽列中，選取**帳戶** > **管理** > **審核日誌**，以存取審核日誌。

審核日誌一開始會顯示帳戶上使用者所採用的最後 25 個互動。您隨時可檢視多達 200 個互動。更新**顯示**下拉清單中顯示的結果數目。如果已變更設定，則互動的**動作**直欄會包含鏈結。按一下任何鏈結，以檢視動作所影響的設定以及變更的詳細資料。按一下任何互動的裝置名稱或使用者名稱，會將您重新導向至裝置詳細資料畫面或使用者設定檔畫面。

### 檢視使用者的存取日誌
{: #cp_viewuserlogs}

「存取日誌」會顯示特定客戶入口網站使用者所進行之每一次存取嘗試的資料。日誌會顯示每一次存取嘗試的日期和時間戳記以及 IP 位址。請使用下列步驟，以檢視使用者的「存取日誌」。

1. 使用唯一的認證來存取[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 從功能表列中，選取**帳戶** > **使用者**，以存取「使用者」視窗。
3. 從**動作**下拉清單中，選取**檢視審核日誌**，以檢視使用者的存取日誌。

每一位使用者的存取日誌都會顯示該使用者按日期進行的存取嘗試，以及進行存取嘗試的 IP 位址。存取日誌內的資訊是唯讀的，因此，任何時間都無法編輯內容。您隨時都可以重複先前的步驟，來重新檢視存取日誌。若要結束日誌並回到「使用者」畫面，請按一下**檢視所有使用者**鏈結。
