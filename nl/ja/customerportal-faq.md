---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# FAQ
{: #bicpfaq}

インフラストラクチャー・リソースの管理の問題に関連してよくある質問を以下に示します。
{:shortdesc}


## カスタマー・ポータルの自分の資格情報を取得するには、どのようにすればよいですか?
{: #bicp_retcreds}

認証に IBM ID を使用する場合は、初めて注文したとき、またはアカウントにユーザーとして追加されたときに、IBM ID を使用して開始するためのリンクが入った E メールが送信されます。 ユーザー名またはパスワードを紛失した、または忘れた場合は、[IBM ID のプロファイル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} に移動して、サインイン・プロセスの後に続く手順を使用してパスワードをリセットするか、復旧してください。 詳細情報の入力が求められます。これには、セキュリティーのための質問への回答が含まれる場合もあります。

認証に IBM ID を使用しない場合は、初めて注文したとき、または[カスタマー・ポータル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} のアカウントにユーザーとして追加されたときに、カスタマー・ポータルで作業を開始するためのユーザー名と初期パスワードが入った E メールを受け取ります。 最初にログインしたら必ず、ユーザー・プロファイルを編集してパスワードを変更してください。 パスワードを変更するには、E メール内の情報を使用してログインし、先頭パネルでユーザー名をクリックしてプロファイルを編集します。

ログイン後にパスワードを忘れた場合は、[カスタマー・ポータル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} のログイン画面にある**「パスワードを忘れた場合」**の機能を使用します。 ユーザー・プロファイルのセットアップ時に指定した一連のセキュリティーのための質問など、特定の情報を入力するよう求めるプロンプトが出されます。

ユーザー名を忘れた場合は、ユーザー名を取得できる、アカウント管理者またはマスター・ユーザーに問い合わせてください。 自分がアカウントの管理者またはマスター・ユーザーである場合は、サポートに連絡して支援を受けてください。

## IBM ID とは何ですか? {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・ユーザーとどう関係していますか?
{: #bicp_whatisibmid}

新規アカウントには、認証のために IBM ID が必要です。 既存アカウントは、マイグレーション・ツールを実行して IBM ID に切り替えるまで、SoftLayer のユーザー名とパスワードを引き続き認証に使用します。 SoftLayer アカウントにはマスター・ユーザーが含まれます。マスター・ユーザーには、同一アカウント内のユーザーを追加する権限があります。 詳しくは、[カスタマー・ポータルにおける SoftLayer アカウントの管理方法 (How SoftLayer accounts are managed in customer portal)](/docs/customer-portal/cphowacctsman.html) を参照してください。

## 既存の SoftLayer アカウントをリンクするには、どのようにすればよいですか?
{: #bicp_linkbmxacct}

SoftLayer アカウントのマスター・ユーザーである場合は、カスタマー・ポータルにログインし、ヘッダーにある**「アカウントのリンク (Link an account)」**をクリックします。  詳しくは、[IBM ID ユーザー・アカウントのリンク](/docs/account/softlayerlink.html)を参照してください。

## アカウントにリンクするには、既存の {{site.data.keyword.Bluemix_notm}} ユーザーである必要がありますか?
{: #bicp_bmxusertolink}

いいえ。新規の {{site.data.keyword.Bluemix_notm}} アカウントを作成するか、既存の {{site.data.keyword.Bluemix_notm}} トライアル・アカウントまたは従量課金 (PAYG) アカウントをリンクできます。


## 2 要素認証はどのように機能しますか?
{: #bicp_2fa}

アカウント・レベルで 2 要素認証構成に影響は全くありません。 2 要素認証は、IBM ID 単位ではなく、依然としてアカウント単位です。 IBM ID が複数のアカウントに関連付けられていて、アカウント間で切り替えを行う場合、2 要素認証を必要とする別のアカウントに切り替えるたびに ID を確認する必要があります。 これは、前のアカウントと新しいアカウントが両方とも同じ 2FA メカニズムを使用して構成されている場合でも同じです。

2 要素認証を使用した IBM ID について詳しくは、[リンクされたアカウントでの 2 要素認証の使用](/docs/account/softlayerlink.html)を参照してください。


## アカウントをリンクできるのは誰ですか?
{: #bicp_wholinkaccts}

SoftLayer アカウントと {{site.data.keyword.Bluemix_notm}} アカウントをリンクできるのは、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・マスター・ユーザーだけです。 マスター・ユーザーの E メールが、リンクされる {{site.data.keyword.Bluemix_notm}} アカウントの基本所有者に関連付けられることも必要です。


## 何を使用して各ポータルにログインしますか?
{: #bicp_logineachport}

アカウントの請求処理はリンクされ、SoftLayer アカウントと {{site.data.keyword.Bluemix_notm}} アカウントの間を簡単に移動できますが、アカウント ID は別々のままです。

* アカウントが認証に IBM ID を使用しない場合は、引き続き、SoftLayer の製品およびサービスには SoftLayer ID を使用し、{{site.data.keyword.Bluemix_notm}} の製品およびサービスには IBM ID を使用します。

* アカウントが認証に IBM ID を使用する場合は、IBM ID を使用して SoftLayer アカウントと {{site.data.keyword.Bluemix_notm}} アカウントの両方にアクセスします。


## SoftLayer ユーザー名でログインしようとしてエラーが出ました。なぜですか?
{: #bicp_SLloginerror}

IBM ID に切り替えた後、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・ユーザー名でカスタマー・ポータルにログインすると、*「無効なログイン資格情報が提供されました」* のエラーが表示されます。
これは、IBM ID に切り替えた後は、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・ユーザー名でカスタマー・ポータルにログインすることはできなくなるためです。 必ず、「アカウントのログイン」ダイアログで**「IBM ID でログイン」**をクリックしてください。

## IBM ID でサインインしようとしてエラーが出ました。なぜですか?
{: #bicp_IBMidloginerror}

IBM ID でサインインする際に、*「この IBMid または E メールを認識できません」* のエラーが出る場合は、完全修飾 E メール・アドレスを入力していることを確認してください。 また、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・ユーザー名を使用していないことも確認してください。


##  認証に IBM ID を使用する新規の SoftLayer アカウントを持っています。{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーと {{site.data.keyword.Bluemix_notm}} の両方に同じ ID を使用できますか?
{: #bicp_loginIBMidSLBlusame}

はい。{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーと {{site.data.keyword.Bluemix_notm}} に 同じ IBM ID でログインできます。


## {{site.data.keyword.Bluemix_notm}} アカウントをリンクしました。私の他の {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・チーム・メンバーにアクセス権限を付与するには、どのようにすればよいですか?
{: #bicp_linkgiveteamaccess}

チーム・メンバーを {{site.data.keyword.Bluemix_notm}} に招待する必要があります。 {{site.data.keyword.Bluemix_notm}} ユーザー・インターフェースで、**「アカウントとサポート」**>**「アカウント」**>**「チーム・メンバーの招待」**を選択します。 リソース・グループを選択すると、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・チーム・メンバーを追加するオプションが表示されます。 招待を送信するには、その前に {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーへのログインが必要な場合があります。 {{site.data.keyword.Bluemix_notm}} は {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・ユーザーのリストを取得します。その後、{{site.data.keyword.Bluemix_notm}} アカウントに招待するユーザーを選択できます。


## IBM ID への切り替え完了の E メールはどこにありますか?
{: #bicp_ibmidswitchemail}

ウィザードに従って IBM ID に切り替えを行って、E メールを受け取っていない場合、登録コードを含む E メールが送信されるまで、数分から数時間かかることがあります。 カスタマー・ポータルの**「ユーザー・プロファイルの編集」**ページに戻って**「E メールの再送」**をクリックし、再試行することが可能です。


## 自分のアカウントには、すべての root アクセス権限がありますか?
{: #bicp_fullrootaccaccess}

マスター・ユーザーと、管理者許可を持つユーザーは、カスタマー・ポータルおよび API でアカウントに対してすべての root アクセス権限を持っています。 管理者許可を持たないユーザーは、管理役割を持つユーザーの制御に従ったアクセス権限を持ちます。 管理者は[ユーザー・プロファイルの編集](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile)によって、カスタマー・ポータルからこれらの許可を更新できます。 管理者許可がなくても、先頭パネルで自分のユーザー名をクリックすることによって、カスタマー・ポータルで自分のユーザー・プロファイルを編集できます。


## {{site.data.keyword.Bluemix_notm}} サブスクリプション・アカウントをリンクできますか?
{: #bicp_linkbmxsubacct}

{{site.data.keyword.Bluemix_notm}} でリンクされるアカウントはすべて、従量課金 (PAYG) アカウントでなければなりません。 新規従量課金 (PAYG) アカウントを作成するか、既存の従量課金 (PAYG) アカウントをリンクできます。 あるいは、既存のトライアル・アカウントをリンクすることもできますが、そのアカウントは従量課金 (PAYG) アカウントにアップグレードされます。


## 自分の {{site.data.keyword.Bluemix_notm}} アカウントと {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・アカウントのリンクを解除するには、どのようにすればよいですか?
{: #bicp_unlinkacct}

リンクされたアカウントをリンク解除することはできません。


## 会社のプロファイルとは何ですか? どこで確認できますか?
{: #bicp_whatfindcompprof}

会社のプロファイルは、アカウント作成時に送信した情報です。会社名、住所、電話番号とともに、会社の主要な連絡先が含まれています。 この情報は、さまざまな理由で使用されるため、常に最新に維持してください。 アカウントの会社のプロファイルを表示する場合、または変更を依頼する場合は、[会社プロファイルの更新](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch) を参照してください。

## デバイスとソフトウェアのパスワードはどこにありますか?
{: #bicp_devswpw}

デバイスとソフトウェアのパスワードは、[カスタマー・ポータル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 内の 2 つの場所に保管されています。 {{site.data.keyword.baremetal_short}} と {{site.data.keyword.virtualmachinesshort}} の両方の root ユーザーまたは管理ユーザーのユーザー名とパスワードなど、デバイスの資格情報を取得するには、[スナップショット・ビュー内でのデバイスの操作
](/docs/vsi/vsi_interact_device_snapshot_view.html)を参照してください。 カスタマー・ポータルを使用して手動で追跡されたソフトウェア資格情報を迅速に表示および取得するには、[デバイス・アクセスの管理](/docs/vsi/vsi_device_access.html)を参照してください。

## Web データの同期を維持するには、どのようにすればよいですか?
{: #bicp_webdatasync}

実サーバー間のデータ整合性の維持はお客様の責任ですが、{{site.data.keyword.BluSoftlayer_full}} では、使用料金が発生せずに同期に使用できるプライベート・ネットワークが提供されています。


## Event Management System とは何ですか?
{: #bicp_whatisems}

Event Management System は、インフラストラクチャーの計画外の問題と近く予定されているメンテナンス・イベントについて、{{site.data.keyword.BluSoftlayer_full}} がユーザーと情報を共有する方法を最適化するツール・セットです。 こうしたインシデントに関して、ターゲットを特定したサブスクリプション・ベースの E メール・アラートを使用して、発生したイベント・タイプを共有します。 イベントの全体的な影響と、進行中の計画外インシデント (UIP) の現行状況に関する追加詳細をサブスクライブ・ユーザーに提供します。

## デバイスをキャンセルするには、どこでどのようにすればよいですか?
{: #bicp_candev}

デバイスのキャンセルは、[カスタマー・ポータル ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} でいつでも行えます。 キャンセル要求の実行について詳しくは、[デバイスのキャンセル](/docs/vsi/vsi_managing.html)に関する箇所を参照してください。
