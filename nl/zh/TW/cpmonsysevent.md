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



# 監視 {{site.data.keyword.Bluemix_notm}} 基礎架構系統事件
{: #customerportal_monevent}

您可以監視系統事件，讓系統流暢地執行。如需在 {{site.data.keyword.BluSoftlayer_full}} 基礎架構中設定及管理虛擬伺服器的相關資訊，請參閱[開始使用虛擬伺服器](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers)。
{:shortdesc}

## 檢視帳戶的審核日誌
{: #cp_viewacctauditlog}

每一個客戶入口網站帳戶都會隨附審核日誌，以追蹤客戶入口網站內每一位使用者的互動。已追蹤的互動包括登入嘗試（成功及失敗）、埠速度更新、開啟或關閉電源和重新開機，以及 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構支援人員所進行的互動。請使用下列步驟，以檢視使用者帳戶的審核日誌。

1. 使用唯一的認證來存取[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 從導覽列中，選取**帳戶** > **管理** > **審核日誌**，以存取審核日誌。

審核日誌一開始會顯示帳戶上使用者所採用的最後 25 個互動。您在任何時間最多都可以檢視 200 個互動。更新**顯示**下拉清單中顯示的結果數目。如果已變更設定，則互動的**動作**直欄將包含鏈結。按一下任何鏈結，以檢視動作所影響的設定以及變更詳細資料。按一下任何互動的裝置名稱或使用者名稱，分別會將您重新導向至裝置詳細資料畫面或使用者設定檔畫面。

## 檢視使用者的存取日誌
{: #cp_viewuserlogs}

「存取日誌」會顯示特定客戶入口網站使用者所進行之每一次存取嘗試的資料。日誌會顯示每一次存取嘗試的日期和時間戳記以及 IP 位址。請使用下列步驟，以檢視使用者的「存取日誌」。

1. 使用唯一的認證來存取[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 從功能表列中，選取**帳戶** > **使用者**，以存取「使用者」視窗。
3. 從**動作**下拉清單中，選取**檢視審核日誌**，以檢視使用者的存取日誌。

每一位使用者的存取日誌都會顯示該使用者按日期進行的存取嘗試，以及進行存取嘗試的 IP 位址。存取日誌內的資訊是唯讀的，因此，任何時間都無法編輯內容。您隨時都可以重複先前的步驟，來重新檢視存取日誌。若要結束日誌並回到「使用者」畫面，請按一下畫面頂端的**檢視所有使用者**鏈結。
