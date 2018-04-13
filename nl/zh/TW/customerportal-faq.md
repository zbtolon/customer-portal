---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-07"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 常見問題 (FAQ)
{: #bicpfaq}

下列常見問題與管理基礎架構資源問題相關。
{:shortdesc}


## 如何擷取客戶入口網站的認證？
{: #bicp_retcreds}

如果您使用 IBM ID 進行鑑別，則當您第一次下單或將您新增為帳戶的使用者時，會傳送一封電子郵件，內含開始使用 IBM ID 的鏈結。如果遺失或忘記您的使用者名稱或密碼，請前往 [IBM ID 設定檔 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window}，並使用登入處理程序後的指示來重設或回復密碼。系統將提示您輸入特定資訊（這可能包括提供安全問題的回答）。

如果您未使用 IBM ID 進行鑑別，則當您第一次下單或將您新增為[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 帳戶的使用者時，會收到一封電子郵件，內含您的使用者名稱及起始密碼，以在客戶入口網站中開始使用。請務必在第一次登入之後變更密碼，方法是[編輯使用者設定檔](edit-user-profile.html)。

如果您在登入之後忘記密碼，請使用[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 登入畫面上所提供的**忘記密碼**特性。系統將提示您輸入特定資訊（這包括您在[編輯使用者設定檔](edit-user-profile.html)時指定的一組安全問題）。

如果您忘記使用者名稱，請聯絡可擷取使用者名稱的帳戶管理者或主要使用者。如果您是帳戶上的管理者或主要使用者，請與支援中心聯絡以取得額外的協助。

## 何謂 IBM ID，以及其與「{{site.data.keyword.BluSoftlayer_notm}} 基礎架構」使用者的關係？
{: #bicp_whatisibmid}

新的帳戶需要 IBM ID 才能進行鑑別。現有帳戶會繼續使用 SoftLayer 使用者名稱及密碼進行鑑別，直到您可以執行移轉工具來切換至 IBM ID。您 SoftLayer 帳戶的主要使用者接著會具有在該相同帳戶內新增其他使用者的權限。如需相關資訊，請參閱[在客戶入口網站中如何管理 SoftLayer 帳戶](/docs/customer-portal/cphowacctsman.html)。

## 如何鏈結現有 SoftLayer 帳戶？
{: #bicp_linkbmxacct}

如果您是 SoftLayer 帳戶上的主要使用者，請登入客戶入口網站，然後按一下標頭中的**鏈結帳戶**。如需相關資訊，請參閱[鏈結 IBM ID 使用者帳戶](/docs/account/softlayerlink.html)。

## 我必須是現有 {{site.data.keyword.Bluemix_notm}} 使用者才能鏈結帳戶嗎？
{: #bicp_bmxusertolink}

否。您可以建立新的 {{site.data.keyword.Bluemix_notm}} 帳戶，或鏈結現有 {{site.data.keyword.Bluemix_notm}} 試用或隨收隨付制帳戶。


## 雙因子鑑別如何運作？
{: #bicp_2fa}

不會影響位於帳戶層次的雙因子鑑別配置。雙因子鑑別不是根據 IBM ID；它仍是根據帳戶。如果 IBM ID 與許多帳戶相關聯，而且您在帳戶之間切換，則每次切換至需要雙因子鑑別的不同帳戶時都必須確認身分。即使前一個帳戶及新的帳戶都已配置相同的雙因子鑑別機制時也是如此。

如需含雙因子鑑別的 IBM ID 的相關資訊，請參閱[已鏈結帳戶中的雙因子鑑別使用](/docs/account/softlayerlink.html)。


## 誰可以鏈結帳戶？
{: #bicp_wholinkaccts}

只有 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構主要使用者才能鏈結 SoftLayer 及 {{site.data.keyword.Bluemix_notm}} 帳戶。主要使用者的電子郵件也必須與所鏈結 {{site.data.keyword.Bluemix_notm}} 帳戶的主要擁有者相關聯。


## 將使用什麼來登入每一個入口網站？
{: #bicp_logineachport}

會鏈結您的帳戶計費，而且您可以輕鬆地在 SoftLayer 與 {{site.data.keyword.Bluemix_notm}} 帳戶之間移動，但您的帳戶身分仍然不同。

* 如果您的帳戶未使用 IBM ID 進行鑑別，請繼續將 SoftLayer ID 用於 SoftLayer 產品及服務，並將 IBM ID 用於 {{site.data.keyword.Bluemix_notm}} 產品及服務。

* 如果您的帳戶使用 IBM ID 進行鑑別，則會使用 IBM ID 來存取 SoftLayer 及 {{site.data.keyword.Bluemix_notm}} 帳戶。


## 我嘗試使用 SoftLayer 使用者名稱登入，但為什麼收到錯誤？
{: #bicp_SLloginerror}

在您切換至 IBM ID 之後，如果使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用者名稱來登入客戶入口網站，則會看到*提供的登入認證無效* 錯誤。原因是，在您切換至 IBM ID 之後，就無法再使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用者名稱來登入客戶入口網站。您必須按一下「帳戶登入」對話框中的**使用 IBM ID 登入**。

## 我嘗試使用 IBM ID 登入，但為什麼收到錯誤？
{: #bicp_IBMidloginerror}

使用 IBM ID 登入時，如果您收到*無法辨識此 IBM ID 或電子郵件* 錯誤，則請確定您輸入的是完整電子郵件位址。也請確定您不是使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用者名稱。


##  我的新 SoftLayer 帳戶使用 IBM ID 進行鑑別；我可以將相同的 ID 用於 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構及 {{site.data.keyword.Bluemix_notm}}？
{: #bicp_loginIBMidSLBlusame}

是的，您可以使用相同的 IBM ID 來登入 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構及 {{site.data.keyword.Bluemix_notm}}。


## 我已鏈結 {{site.data.keyword.Bluemix_notm}} 帳戶，如何將存取權提供給其他 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構團隊成員？
{: #bicp_linkgiveteamaccess}

您必須邀請他們加入 {{site.data.keyword.Bluemix_notm}}。在 {{site.data.keyword.Bluemix_notm}} 使用者介面中，選取**帳戶及支援** > **帳戶** > **邀請團隊成員**。在您選取資源群組之後，會看到新增 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構團隊成員的選項。您需要先登入 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構，才能傳送邀請。{{site.data.keyword.Bluemix_notm}} 會取得 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用者清單，然後，您可以選取要邀請加入 {{site.data.keyword.Bluemix_notm}} 帳戶的使用者。


## 完成切換至 IBM ID 的電子郵件在哪裡？
{: #bicp_ibmidswitchemail}

如果您已遵循切換至 IBM ID 的精靈，但未收到電子郵件，則可能是需要數分鐘到數小時的時間才會送出含登錄碼的電子郵件。您可以回到客戶入口網站中的**編輯使用者設定檔**頁面，然後按一下**重新傳送電子郵件**以重試。


## 我具有我帳戶的完整 root 存取權嗎？
{: #bicp_fullrootaccaccess}

主要使用者及具有管理者許可權的使用者都會有客戶入口網站及 API 上帳戶的完整 root 存取權。沒有管理者許可權的使用者的可存取性是由具有 admin 角色的使用者所控制。您可以藉由在客戶入口網站中[編輯使用者設定檔](edit-user-profile.html)，以隨時更新這些許可權。


## 我可以鏈結 {{site.data.keyword.Bluemix_notm}} 訂閱帳戶嗎？
{: #bicp_linkbmxsubacct}

{{site.data.keyword.Bluemix_notm}} 中的所有已鏈結帳戶都必須是隨收隨付制帳戶。您可以建立新的隨收隨付制帳戶，或鏈結現有隨收隨付制帳戶。或者，您可以鏈結現有試用帳戶，但它將會升級成隨收隨付制帳戶。


## 如何解除 {{site.data.keyword.Bluemix_notm}} 帳戶與 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構帳戶的鏈結？
{: #bicp_unlinkacct}

帳戶在鏈結之後，即無法解除鏈結。


## 何謂公司設定檔以及可以在哪裏找到它？
{: #bicp_whatfindcompprof}

公司設定檔就是建立帳戶時所提交的資訊，包括公司的主要聯絡人，以及公司名稱、地址及電話號碼。這項資訊的使用原因眾多，應該隨時保持為最新。若要檢視您帳戶的公司設定檔，或要求變更，請參閱[更新公司設定檔](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch)。

## 在哪裏可以找到我的裝置及軟體密碼？
{: #bicp_devswpw}

裝置及軟體密碼儲存在[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 內的兩個位置。若要擷取裝置認證（包括 {{site.data.keyword.baremetal_short}} 及 {{site.data.keyword.virtualmachinesshort}} 的 root 或管理使用者名稱及密碼），請參閱[在 Snapshot 視圖中與裝置互動](/docs/vsi/vsi_interact_device_snapshot_view.html)。若要快速檢視及擷取使用客戶入口網站手動追蹤的軟體認證，請參閱[管理裝置存取權](/docs/vsi/vsi_device_access.html)。

##如何保持 Web 資料同步？
{: #bicp_webdatasync}

雖然您負責維護實際伺服器之間的資料一致性，但是 {{site.data.keyword.BluSoftlayer_full}} 提供您可用來同步化而不會產生使用費用的專用網路。


## 何謂事件管理系統？
{: #bicp_whatisems}

「事件管理系統」是一個工具集，可最佳化 {{site.data.keyword.BluSoftlayer_full}} 與使用者共用有關非計劃性基礎架構問題及即將到來的計劃性維護事件的資訊的方式。它會使用已設定目標的訂閱型電子郵件警示，讓這些突發事件共用所發生事件的類型。它會將整體事件影響以及進行中非計劃性突發事件 (UIP) 的現行狀態的其他詳細資料提供給已訂閱使用者。

## 取消裝置的方式及位置為何？
{: #bicp_candev}

您隨時可以透過[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 來取消裝置。如需完成取消要求的相關資訊，請參閱[取消裝置](/vsi/vsi_managing.html)。
