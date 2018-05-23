---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-26"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# シングル・サインオンの構成
{: #customerportal_confssoserv}

アカウントのマスター・ユーザーであるか、アカウントへの管理アクセス権限を持っている場合、シングル・サインオンを構成できます。 {{site.data.keyword.BluSoftlayer_full}} インフラストラクチャーのシングル・サインオンの構成は、2 つのステップからなるプロセスです。  最初に、ID プロバイダーを選択してセットアップします。 次に、ID プロバイダーから認証要求を受け取るように {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーをセットアップします。
{:shortdesc}

## ID プロバイダーの選択とセットアップ
{: #cp_setupidprov}

まだ ID プロバイダーを持っていない場合、まず ID プロバイダーを選択してセットアップします。 {{site.data.keyword.BluSoftlayer_notm}} と共に使用できる ID プロバイダーは次のとおりです。
* Ping Identity&reg;
* OneLogin&trade;
* IBM&reg; Cloud Security Enforcer
* IBM Cloud Identity Services。
詳しくは、{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーの営業担当員にお問い合わせください。

まだ ID プロバイダーをセットアップしていない場合、ID プロバイダーのサポートに連絡して具体的な手順を確認するか、または、以下の手順概要を使用して ID プロバイダーを構成します。
1. ID プロバイダー環境を、実行可能ファイルをダウンロードおよびインストールすることによって作成します。
2. {{site.data.keyword.BluSoftlayer_notm}} 認証と連携して機能するよう ID プロバイダーを構成します。

## SSO のための {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーのセットアップ
{: #cp_setupsso}

{{site.data.keyword.BluSoftlayer_notm}} と共に使用するため、Security Assertion Markup Language&trade; (SAML&trade;) 2.0 メタデータ情報の以下の必須フィールドを ID プロバイダーから抽出する必要があります。
<dl>
<dt>エンティティー ID</dt>
<dd>ID プロバイダーのエンティティー ID。</dd>
<dt>シングル・サインオン URL</dt>
<dd>SSO のための ID プロバイダーのエンドポイント。</dd>
<dt>証明書</dt>
<dd>要求に署名するために使用される、ID プロバイダーの証明書。</dd>
</dl>

以下のフィールドはオプションです。
<dl>
<dt>証明書指紋</dt>
<dd>証明書の指紋。 証明書全体の代わりにこのフィールドを使用できます。</dd>
</dl>

以下の手順を使用して、ID プロバイダーから認証要求を受け取るように {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーをセットアップします。
1. まだログインしていない場合は ID プロバイダーにログインし、**「SAML 構成 (SAML configuration)」**ページを見つけます。 以下の情報をメモします。
  * エンティティー ID
  * シングル・サインオン URL
  * 証明書 (これは、ご使用の ID プロバイダーによって異なります)
2. SoftLayer アカウントの作成に使用したマスター・ユーザー名とパスワードを使用して、マスター・ユーザーとして {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーにログインします。
3. **「アカウント」** > **「管理」** > **「SAML 認証 (SAML Authentication)」**をクリックします。
4. **「ID プロバイダー (Identity Provider)」**メタデータを入力します。
5. **「保存」**をクリックします。
6. **「アカウント」** > **「管理」** > **「SAML 認証 (SAML Authentication)」**をクリックします。
7. **「XML 構成のダウンロード (Download XML Configuration)」**をクリックして、サービス・プロバイダー・メタデータをダウンロードするか、情報をメモします。
8. **「サービス・プロバイダー (Service Provider)」**メタデータを使用して、ご使用の ID プロバイダーの指示に基づいて ID プロバイダーを構成します。  

これで、フェデレーテッド ID を使用して {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーにログインできるようになりました。 フェデレーテッド ID について詳しくは、[{{site.data.keyword.Bluemix_notm}} への登録](/docs/account/adminpublic.html)および[IBMid Enterprise Federation Adoption Guide ![外部リンク・アイコン](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}を参照してください。
