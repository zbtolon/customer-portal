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

# Utilisation de comptes IBMid avec l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}
{: #customerportal_ibmid}

Désormais, l'authentification dans l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} utilise l'IBMid afin de fournir une connexion unique pour {{site.data.keyword.Bluemix_notm}}.
{:shortdesc}

Si
vous possédez un compte SoftLayer, vous pouvez passez à un IBMid. Un assistant de migration peut vous guider tout au long de cette opération. Pour plus d'informations, voir [Passage à l'IBMid](/docs/account/softlayerlink.html#switching-to-ibmid).

## Mappage de plusieurs comptes SoftLayer à un IBMid
{: #cp_mapmultclinfrto1ibmid}

Vous pouvez associer un IBMid à plusieurs comptes SoftLayer en utilisant une adresse électronique IBMid existante lorsque vous configurez le
compte. Vous ne pouvez mapper qu'un seul utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour chaque compte à l'IBMid unique. L'IBMid doit être unique dans chaque compte SoftLayer. Toutefois, un utilisateur avec accès à plusieurs comptes SoftLayer peut utiliser un même IBMid pour accéder à ces comptes.

Par exemple, un IBMid peut être mappé à l'utilisateur principal dans les comptes A et B, et à un autre utilisateur dans les comptes C et D. L'un des comptes mappés à cet IBMid constitue le compte par défaut. En général, le compte par défaut est celui qui a été mappé en premier à l'IBMid. Toutefois, vous pouvez changer le compte par défaut à l'aide d'une fonction à cet effet dans le portail client.

![Mappage de comptes SoftLayer à un IBMid](images/ibmid-image.png)

Pour un utilisateur disposant d'un accès IBMid à plusieurs comptes pour lesquels l'authentification à deux facteurs (2FA) est activée, un code de vérification 2FA est requis. Le code de vérification est requis, par compte, lors de la connexion au compte et lorsque vous changez de compte par défaut.
