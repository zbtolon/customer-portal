---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 設定裸機伺服器
{: #customerportal_setupbaremetal}

您可以將「裸機伺服器」設定為專用伺服器。
{:shortdesc}

請使用下列步驟，以設定「裸機伺服器」：

1. 使用唯一的認證來登入 {{site.data.keyword.BluSoftlayer_full}} 客戶入口網站。

2. 從功能表上，按一下**裝置** > **裝置清單**來尋找您的系統。您的所有裝置都會詳述於「裝置清單」，在其中，您可以管理裝置、升級裝置，或產生頻寬用量圖表。

3. 選擇以下列其中一種方式管理伺服器：
  * 按一下「裝置名稱」旁的箭頭，以從 Snapshot 視圖檢視摘要及管理裝置。
  * 按一下伺服器的「裝置名稱」，以從「裝置詳細資料」畫面檢視詳細清單及管理裝置。

4. 將伺服器的 IP 位址及認證記錄在安全的位置，以便快速存取詳細資料，而無需在每次需要時登入「客戶入口網站」。您可以針對個別裝置及與您帳戶相關聯的所有裝置，記錄這些詳細資料：
  * 從「裝置清單」檢視個別裝置 IP。
  * 在裝置的「Snapshot 視圖」中檢視個別裝置 root 密碼。
  * 使用**裝置清單**中的**下載 CSV** 選項來檢視多個裝置 IP。然後，從**設定**齒輪選取**下載 CSV**，以試算表格式下載裝置及詳細資料的完整清單。

5. 更新作業系統及其他軟體的認證。會指派暫時認證給在佈建處理程序期間載入到裝置上的所有軟體。您可以在「客戶入口網站」中，在每個裝置的「密碼」標籤上檢視及管理這些認證。第一次時使用這些暫時認證來存取您的軟體，然後使用由字母、數字及符號的組合構成的高保護性密碼變更軟體的密碼。您可以選擇在「密碼」標籤上儲存每台裝置的密碼更新。當您在客戶入口網站中儲存密碼時，任何具有帳戶存取權及適當許可權的人員都可以在「密碼」畫面上檢視已儲存的密碼。

6. 存取專用網路上的伺服器。您可以透過使用 SSH 及 KVM over IP 搭配遠端桌面 (RDP)，使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構專用網路來與您的裝置互動。您可以使用「VPN 存取權」工具來進行專用網路連線，來連至最近的 SSL VPN 端點或是您所選擇的端點。與數個服務進行互動時也需要 VPN 存取權。若要存取專用網路，請從「使用者清單」編輯使用者的 VPN 存取權。若要存取「使用者清單」，請按一下**帳戶** > **使用者** > **使用者清單**。使用[虛擬專用網路 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://www.softlayer.com/VPN-Access){:new_window} 頁面，以連接至各種 VPN 選項的其中一個。

7. 設定監視來檢查伺服器的狀態，以瞭解何時需要擴充。您可以使用標準監視或 Nimsoft 監視服務。您可以透過在客戶入口網站中使用慢速或服務連線測試，以連線測試及回應 (ping-and-respond) 方法進行標準（或基本）監視。您也可以使用客戶入口網站中的 Nimsoft（或進階）監視，或是在下列三層其中之一進行監視：基本、進階及超值。

8. 保護您的系統。請使用可用的硬體防火牆來確保您的裝置隨時都是安全的。如果已適當地建立規則，您可以隨需應變建立硬體防火牆而不會有關閉時間，以保護您的伺服器免於進行不想要的活動。訂購防火牆之後，必須加以啟用並設定規則。

9. 排定備份以確保您的資料安全地儲存於裝置之外，且能在資料遺失時重新載入。您可以從各種備份服務選擇，將您的資料儲存在安全的位置：
  * EVault Backup 是一種自動化、代理程式型的備份系統。這是用於管理裝置的熱門「設定後即忘記」解決方案。它透過其他外掛程式而與 Microsoft 軟體（包括 Exchange 和 SQL）相容。EVault 使用者可以透過 EVault 的 WebCC Web 型應用程式與此服務進行互動。
  * R1Soft Continuous Data Protection (CDP) 可以安裝在您的伺服器或自我管理的虛擬機器上。如果您要尋找的是以單一介面來管理所有的備份，則建議使用此產品。您可透過專有管理系統與 R1Soft CDP 互動，而此管理系統容許代理程式安裝在虛擬機器上，並且會提供資料庫外掛程式來提供更多功能。
