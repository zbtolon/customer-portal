---

copyright:

  years: 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 設定雙因子鑑別
{: #customerportal_2fa}

在客戶入口網站中，可以啟動外部雙因子鑑別 (2FA)，為您登入入口網站時增加額外的保護。這個額外安全層可保護帳戶不受未驗證地存取，確保裝置、資料及帳戶資訊受到保護。
{:shortdesc}

如果您在客戶入口網站中為 SoftLayer 帳戶啟用 2FA，在您登入 {{site.data.keyword.Bluemix_notm}} 主控台時，需要輸入安全碼。2FA 只適用於 {{site.data.keyword.Bluemix_notm}} 帳戶中的基礎架構資源。您可以對 {{site.data.keyword.Bluemix_notm}} 帳戶中的資源執行各種動作，而不必完成 2FA。

SoftLayer 帳戶的 2FA 不是根據 IBM ID。它仍是根據帳戶。當 IBM ID 與多個帳戶相關聯，且您在帳戶之間切換時，每次切換到不同帳戶時都必須確認身分。即使前一個帳戶及新的帳戶都已配置相同的雙因子鑑別機制，您也必須在切換帳戶時確認您的身分。

## 啟用 2FA

2FA 鑑別以兩種形式提供。兩種外部鑑別方法都可以為每位使用者新增，只需要少量的每月費用：

* Symantec Identify Protection 是最常用的外部鑑別工具，在您存取客戶入口網站時，除了使用者名稱及密碼之外，還會提供所使用的動態安全碼。
* PhoneFactor 鑑別透過通話、SMS 或行動應用程式來提供頻外鑑別。

 如果您具有已鏈結帳戶，則可以藉由為您的整個 {{site.data.keyword.Bluemix_notm}} 帳戶[啟用多因子鑑別](/docs/iam/mfa.html)，利用多因子鑑別 (MFA) 設定。
 {: tip}

若要設定 2FA，請完成下列步驟：

1. 存取客戶入口網站中的**使用者**畫面。
2. 從使用者的**動作**功能表，選取**新增外部鑑別**。
3. 根據要訂購的外部鑑別類型，完成下列步驟：
    * 如果您選擇 Symantec Identity Protection，請選取 **Symantec Identity Protection**，然後輸入使用者的認證 ID。
    * 如果您選擇 PhoneFactor，請選取 **PhoneFactor**。
4. 按一下**繼續**。
5. 完成畫面上的**促銷代碼**及 **MSA 認可**提示。
6. 按一下**訂購外部鑑別**，以完成訂單。按一下**取消**即可取消動作。

## 後續步驟
{: #2fanextsteps}

在新增使用者的外部鑑別之後，接下來的步驟取決於鑑別類型。
* 如果已啟用 Symantec Identity Protection，則必須新增與使用者「認證 ID」相關聯的安全代碼。此安全代碼是 Symantec Identity Protection 新增至帳戶時在系統中輸入的代碼。
* 如果已啟用 PhoneFactor，則使用者必須啟動 PhoneFactor，以搭配使用這類型的雙因子鑑別與帳戶。

### 啟動 PhoneFactor 鑑別
{: #cp_actphonefacauth}

在新增 PhoneFactor 之後，您必須透過客戶入口網站手動啟動與 PhoneFactor 的外部鑑別。因為 PhoneFactor 使用手動聯絡，所以務必確保與帳戶相關聯的所有電話號碼隨時都是最新資訊。無法持續更新聯絡資訊可能會導致在 PhoneFactor 作用時，無法存取客戶入口網站及 VPN。順利新增 PhoneFactor 之後，您會收到一封電子郵件用來確認已新增 PhoneFactor。在收到電子郵件之後，請使用下列步驟來啟動 PhoneFactor 鑑別。

1. 使用唯一的認證來存取客戶入口網站。
2. 從導覽列中，選取**帳戶 > 使用者**。
3. 按一下使用者名稱，以存取該使用者的關聯使用者設定檔。
4. 捲動至 **PhoneFactor 設定**區段。

  如果「PhoneFactor 設定」區段無法使用，請先驗證您已收到 PhoneFactor 佈建電子郵件，指出已佈建 PhoneFactor。如果已佈建 PhoneFactord，但是此區段無法使用，請建立支援問題單。如果尚未佈建 PhoneFactor，請等待電子郵件，然後再試一次。
  {: tip}

5. 從**狀態**清單中，選取**作用中**。
6. 編輯進行鑑別的**主要電話號碼**。
  1. 按一下**編輯**鏈結。
  2. 在關聯的欄位中，輸入**國碼**、**電話號碼**及**分機**（適用時）。
  3. 按一下**鑑別並儲存號碼**，以完成鑑別。

    新增進行鑑別的電話號碼時，您必須在電話旁邊。在按一下**鑑別**之後，即會撥打此號碼，而且系統會提示您完成鑑別號碼的步驟。必須完成這些步驟，才能鑑別電話號碼。
    {: tip}

  4. 若要新增**次要電話號碼**，請重複這些步驟。
7. 從**方法**清單中，選取**聯絡方法**。
8. 從 **PIN 碼類型**清單中，選取 **PIN 碼類型**。
9. 如果您選取**一次性** > **PIN 碼值**，請在 **PIN 碼值**欄位中輸入 PIN 碼。
10. 按一下**更新**，以更新變更，並啟動 PhoneFactor 鑑別。

啟動 PhoneFactor 之後，客戶入口網站或 VPN 需要透過 PhoneFactor 進行鑑別。透過使用者認證進行鑑別之後，有一則訊息會告訴您將嘗試進行 PhoneFactor 鑑別。您或所新增的使用者必須在使用 PhoneFactor 所列出的電話旁邊，才能完成鑑別。PhoneFactor 會嘗試鑑別五次。在五次不成功的鑑別嘗試之後，會將您鎖定大約一小時。您或具有帳戶管理存取權的使用者隨時都可以變更 PhoneFactor 鑑別設定。您或帳戶管理者隨時可以取消啟動 PhoneFactor。

 如果您選擇為客戶入口網站和 VPN 登入設定 PhoneFactor，結果便是兩個不同的 2FA 登入處理程序，一個用於客戶入口網站，而另一個用於 VPN。
 {: tip}

#### PhoneFactor 鑑別方法
{: #cp_phonefacauthmeths}

如果您設定 PhoneFactor 作為鑑別類型，則可以選擇下列其中一個選項作為鑑別方法：

<dl>
<dt>通話及標準（無 PIN 碼）</dt>
<dd>如果啟用此選項，您會在登入入口網站時接到撥入已啟用之主要號碼的通話。當您接聽通話時，會要求您按 # 鍵來完成鑑別。</dd>
<dt>使用 PIN 碼的通話</dt>
<dd>如果選取此選項，您會在客戶入口網站中輸入 PIN 碼值。PIN 碼必須是 4 - 8 個數字。當您嘗試登入入口網站時，會接到撥入入口網站中所列主要號碼的通話。當您接聽時，會要求您輸入 PIN 碼，然後按下 #，以完成鑑別。</dd>
<dt>SMS 文字及一次性 PIN 碼</dt>
<dd>如果選取此選項，您會收到含有 PIN 碼的文字訊息，而您可以使用此 PIN 碼來回覆訊息。當您輸入提供的 PIN 碼時，鑑別處理程序會完成，並將您登入入口網站。</dd>
<dt>含有一次性及 PIN 碼值的 SMS 文字</dt>
<dd>如果選取此選項，您會建立 4 - 8 個數字的 PIN 碼值。然後，您會收到一則文字訊息，並以提供的代碼及 PIN 碼（無空格）回覆。</dd>
<dt>PhoneFactor 應用程式及標準（無 PIN 碼）</dt>
<dd>在裝置上開啟 PhoneFactor 應用程式 (Microsoft Authenticator)，然後按一下<strong>鑑別</strong>。它顯示您已使用 PhoneFactor 順利進行鑑別，並將您登入入口網站。</dd>
<dt>使用 PIN 碼的 PhoneFactor 應用程式</dt>
<dd>使用此選項，您可以在入口網站中設定 4 - 8 個數字的 PIN 碼。然後，在裝置上開啟 PhoneFactor 應用程式 (Microsoft Authenticator)。接下來，輸入在入口網站中建立的 PIN 碼，然後按一下<strong>鑑別</strong>以登入入口網站。</dd>
</dl>
