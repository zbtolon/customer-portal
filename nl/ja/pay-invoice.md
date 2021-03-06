---

copyright:

  years: 1994, 2018

lastupdated: "2018-10-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 支払いを行う
{: #customerportal_makepayment}

請求書から支払い情報まで、{{site.data.keyword.Bluemix}} インフラストラクチャー請求処理の詳細はすべて、カスタマー・ポータルに安全に保管されています。 支払い方法を変更する場合、あるいは、クレジット・カードが取り消された、または期限切れになった場合は、支払い情報を更新し、延滞料金が発生しないようにしてください。
{:shortdesc}

## 請求書の表示
{: #cp_viewinvoice}

「請求書」ウィンドウで、個々の請求書は、請求書番号、日付、請求書タイプ、および各種の請求金額によって要約されます。 請求書には、以下のタイプが可能です。

<dl>
<dt>新規</dt>
<dd>繰り返し発生する一連の請求書の最初の請求書。</dd>
<dt>繰り返し</dt>
<dd>複数の月にわたってアカウントでアクティブであった繰り返し発生する料金の請求書。</dd>
<dt>1 回限りの課金</dt>
<dd>各種の費用 (超過分を含む) の 1 回限りの課金。</dd>
<dt>クレジット</dt>
<dd>{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーから勘定残高へのクレジット。</dd>
<dt>返金</dt>
<dd>1 回限りの課金または繰り返し発生する課金の支払い戻し。</dd>
</dl>

アカウントの請求処理の要約を表示することもできます。これには、以下の情報が含まれます。
  * 現在の残高および次回の見積もり残高
  * 支払方法
  * 前回および次回の繰り返し発生する請求書の日付

1. メニューから**「アカウント」**>**「請求処理」**>**「請求書」**をクリックします。
2. カスタマー・ポータルで請求書を表示したり、請求書をダウンロードしたりできます。

カスタマー・ポータルで請求書を表示すると、選択した請求書について、請求項目の明細リストが表示されます。 請求項目の行のどこかをクリックすると、その料金に関する項目別の詳細が表示されます。 請求書をダウンロードすると、ブラウザーの設定に基づいてそれを表示できます。 ダウンロードした請求書には、各請求項目について、項目別の要約と項目別の請求詳細の両方が示されます。

## 支払い方法の追加
{: #cp_cpmanacctbillpay}

各 SoftLayer アカウントには、毎月、請求金額を自動的に課金するクレジット・カードが登録されていなければなりません。 支払いの遅延をなくすため、この情報は常に最新にする必要があります。支払い情報を常に正確にしておくために、この情報はいつでも更新できます。 登録されたクレジット・カード情報は正しいが、現在の残高には別の支払い形式を適用したい場合は、[請求アイテムの管理](/docs/customer-portal/cpmanacctbillpay.html#cp_makeonetimepayment)を参照してください。 カスタマー・ポータルでアカウントの支払い方法を追加するには、以下の手順を使用します。

1. メニューから**「アカウント」**>**「請求処理」**>**「支払い方法」**をクリックします。
2. **「請求先住所」**セクションの各フィールドに、カードの必要な請求処理詳細を入力します。
> **注:** **「会社情報を使用」**チェック・ボックスをクリックすると、当該アカウントについて {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーに登録されている会社情報がフィールドに自動入力されます。
3. **「支払い情報」**セクションの各フィールドに、クレジット・カード情報を入力します。
4. **「クレジット・カードの追加」**をクリックして、このクレジット・カードを毎月の支払い方法として追加します。
5. オプションで、ヨーロッパのサポート・チームがメンテナンスおよびサポートの問題を処理するようにする場合は、**「EU サポート対象 (EU Supported)」**を選択します。  このオプションについて詳しくは、[EU サポート対象オプションの設定](/docs/customer-portal/cpmanuserprof.html#cp_seteusupported)を参照してください。

支払い方法を追加すると、カードの有効性を検証するために、SoftLayer アカウント担当者が要求を処理します。 検証が完了したカードは、24 時間以内にアカウントで使用可能になります。 支払い方法の追加時に指定した連絡先に、支払い方法の状況変更の E メールが送信されます。

## 1 回払を行う
{: #cp_makeonetimepayment}

PayPal アカウントまたは主要なクレジット・カードを使用して、1 回払を行うことができます。また、請求額の全額または一部の支払いを行えます。 1 回払の詳細は、将来使用のために記録されず、アカウントで現行の毎月の支払い方法は変更されません。

1. カスタマー・ポータルで「1 回払を行う」ページに移動します。
 * メニューから、**「アカウント」**>**「支払いを行う」**に移動します。
 * 「請求書」ページで**「残高の支払い」**をクリックします。
2. **「支払い金額」**フィールドに支払い金額を入力します。
3. PayPal で支払いを行う場合は、**「PayPal」**をクリックし、PayPal のプロンプトに従って支払いを完了します。 これ以上のアクションは不要です。 クレジット・カードで支払いを行う場合は、**カード番号、有効期限、セキュリティー・コード**を該当フィールドに入力します。
4. **「クレジット・カードの請求先住所」**セクションの該当フィールドに、請求先情報を入力します。
5. オプションで、ヨーロッパのサポート・チームがメンテナンスおよびサポートの問題を処理するようにする場合は、**「EU サポート対象 (EU Supported)」**を選択します。  このオプションについて詳しくは、[EU サポート対象オプションの設定](/docs/customer-portal/cpmanuserprof.html#cp_seteusupported)を参照してください。
6. **「クレジット・カードでの支払い」**をクリックし、支払いを開始します。

支払いを開始すると、支払いが処理されます。 支払いで問題が発生した場合は、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーまたは PayPal のプロンプトに従って問題を解決してください。 支払いは処理されます。 金額が適用され、現在の残高が更新されます。
