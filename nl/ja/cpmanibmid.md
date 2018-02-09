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

# {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーでの IBM ID アカウントの使用
{: #customerportal_ibmid}

{{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャーでの認証では、{{site.data.keyword.Bluemix_notm}} 用の単一のログインを提供するために IBM ID を使用するようになりました。
{:shortdesc}

既存の SoftLayer アカウントがある場合、IBM ID に切り替えることができます。 この切り替えにはマイグレーション・ウィザードが役立ちます。詳しくは、[IBM ID への切り替え](/docs/account/softlayerlink.html#switching-to-ibmid)を参照してください。

## 単一の IBM ID への複数の SoftLayer アカウントのマップ
{: #cp_mapmultclinfrto1ibmid}

アカウントのセットアップ時に既存の IBM ID の E メール・アドレスを使用することで、単一の IBM ID を複数の SoftLayer アカウントに関連付けることができます。 単一の IBM ID にマップできるのは、アカウントごとに 1 つのみの {{site.data.keyword.BluSoftlayer_notm}} インフラストラクチャー・ユーザーです。IBM ID は、各 SoftLayer アカウント内で固有でなければなりません。 ただし、複数の SoftLayer アカウントにアクセスできる単一のユーザーが、単一の IBM ID を使用して複数の SoftLayer アカウントにアクセスできます。

例えば、ある IBM ID をアカウント A と B のマスター・ユーザーにマップし、さらにアカウント C と D の追加ユーザーにマップできます。当該 IBM ID にマップされたアカウントの 1 つが、デフォルト・アカウントになります。 通常、デフォルト・アカウントは、IBM ID に最初にマップされたアカウントです。 ただし、カスタマー・ポータルのアカウント切り替え機能を使用して、デフォルトのアカウントにするアカウントを切り替えることができます。

![1 つの IBM ID への複数の SoftLayer アカウント](images/ibmid-image.png)

2 要素認証が有効になっていて、複数のアカウントに IBM ID でアクセスできるユーザーの場合、アカウントのログインおよびアカウントの切り替え時に、アカウントごとに適切な 2 要素認証検証コードが必要になります。
