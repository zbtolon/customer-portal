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


# Foire aux questions
{: #bicpfaq}

Les questions les plus fréquentes suivantes sont liées à la gestion des problèmes de ressources d'infrastructure.
{:shortdesc}


## Comment extraire mes données d'identification du portail client ?
{: #bicp_retcreds}

Si vous utilisez IBMid pour l'authentification, lorsque vous validez votre première commande ou que vous êtes ajouté en tant qu'utilisateur à un compte, vous recevez un e-mail comportant un lien pour vous permettre de débuter avec votre IBMid. Si vous perdez ou oubliez votre nom ou votre mot de passe, accédez à votre [profil IBMid ![Icône de lien externe](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} et réinitialisez ou récupérez le mot de passe en suivant les instructions fournies après le processus de connexion. Vous serez invité à entrer des informations spécifiques, lesquelles peuvent inclure des réponses à vos questions de sécurité.

Si vous n'utilisez PAS IBMid pour l'authentification, lorsque vous validez votre première commande ou que êtes ajouté en tant qu'utilisateur à un compte de [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, vous recevez un e-mail contenant votre nom d'utilisateur et votre mot de passe initial pour débuter sur le portail client. Veillez à changer votre mot de passe après vous être connecté pour la première fois en [éditant votre profil utilisateur](edit-user-profile.html).

Si vous oubliez votre mot de passe après votre première connexion, utilisez la fonction de **mot de passe oublié** disponible sur l'écran de connexion du [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Vous serez invité à entrer des informations spécifiques, notamment répondre à un ensemble de questions de sécurité spécifiées lors de l'[édition de votre profil utilisateur](edit-user-profile.html).

Si vous oubliez votre nom d'utilisateur, contactez votre administrateur de compte ou utilisateur principal, qui dispose des droits pour extraire votre nom d'utilisateur. Si vous êtes l'administrateur ou l'utilisateur principal sur le compte, contactez le support pour une aide supplémentaire.

## Qu'est-ce que l'IBMid, et comment est-il associé aux utilisateurs de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} ?
{: #bicp_whatisibmid}

Les nouveaux comptes nécessitent IBMid pour l'authentification. Les comptes existants continuent d'utiliser les nom d'utilisateur et mot de passe SoftLayer pour l'authentification tant que vous n'avez pas exécuté l'outil de migration pour passer à un IBMid. Votre compte SoftLayer possède un utilisateur principal doté des droits d'ajout d'autres utilisateurs au sein de ce même compte. Voir [Gestion des comptes SoftLayer dans le portail client](/docs/customer-portal/cphowacctsman.html) pour plus d'informations.

## Comment lier un compte SoftLayer existant ?
{: #bicp_linkbmxacct}

Si vous êtes l'utilisateur principal sur votre compte SoftLayer, connectez-vous au portail client et cliquez sur **Lier le compte** dans l'en-tête.  Voir [Liaison de comptes utilisateur IBMid](/docs/account/softlayerlink.html) pour plus d'informations.

## Faut-il être un utilisateur {{site.data.keyword.Bluemix_notm}} existant pour lier des comptes ?
{: #bicp_bmxusertolink}

Non. Vous pouvez créer un compte {{site.data.keyword.Bluemix_notm}} ou lier un compte {{site.data.keyword.Bluemix_notm}} d'essai ou de paiement à la carte déjà existant.


## Comment fonctionne l'authentification à deux facteurs ?
{: #bicp_2fa}

Il n'y a pas d'impact sur la configuration de l'authentification à deux facteurs au niveau du compte. L'authentification à deux facteurs ne se fait pas par IBMid mais toujours par compte. Quand un IBMid est associé à de nombreux comptes et que vous passez d'un compte à un autre, vous devez confirmer votre identité chaque fois que vous utilisez un compte différent qui nécessite une authentification à deux facteurs. Ceci est valable même si le compte précédent et le nouveau compte ont tous deux été configurés avec le même mécanisme 2FA.

Pour plus d'informations sur l'IBMid avec authentification à deux facteurs, voir [Utilisation de l'authentification à deux facteurs dans les comptes liés](/docs/account/softlayerlink.html).


## Qui peut lier des comptes ?
{: #bicp_wholinkaccts}

Seuls les utilisateurs principaux de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} peuvent lier des comptes SoftLayer et {{site.data.keyword.Bluemix_notm}}. L'e-mail d'un utilisateur principal doit également être associé au propriétaire principal du compte {{site.data.keyword.Bluemix_notm}} à lier.


## Que dois-je utiliser pour me connecter à chaque portail ?
{: #bicp_logineachport}

La facturation de vos comptes est liée et vous pouvez aisément passer de votre compte SoftLayer à votre compte {{site.data.keyword.Bluemix_notm}} et vice-versa, mais les identités de vos comptes restent distinctes.

* Si votre compte n'utilise pas IBMid pour l'authentification, continuez à utiliser votre ID SoftLayer pour les produits et services SoftLayer et utilisez votre IBMid pour les produits et services {{site.data.keyword.Bluemix_notm}}.

* Si votre compte utilise IBMid pour l'authentification, vous utilisez votre IBMid pour accéder à vos comptes SoftLayer et {{site.data.keyword.Bluemix_notm}}.


## J'ai reçu un message d'erreur en essayant de me connecter avec mon nom d'utilisateur SoftLayer, pourquoi ?
{: #bicp_SLloginerror}

Une fois que vous êtes passé à un IBMid, si vous vous connectez au portail client avec votre nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}, vous voyez s'afficher l'erreur *"Données d'identification incorrectes."*.
Comme vous avez changé pour un IBMid, vous ne pouvez plus vous connecter au portail client avec votre nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Vous devez cliquer sur **Connexion avec identité IBM** dans la boîte de dialogue Connexion au Compte.

## J'ai reçu un message d'erreur en essayant de me connecter avec mon IBMid, pourquoi ?
{: #bicp_IBMidloginerror}

Lorsque vous vous connectez avec votre IBMid, si vous voyer s'afficher l'erreur *"Nous ne reconnaissons pas cet IBMid ou cette adresse électronique."*, vérifiez que vous avez bien entré une adresse e-mail qualifiée complète. Vérifiez également que vous n'utilisez pas votre nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.


##  Je possède un nouveau compte SoftLayer qui utilise IBMid pour l'authentification, puis-je utiliser le même ID pour l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} et {{site.data.keyword.Bluemix_notm}} ?
{: #bicp_loginIBMidSLBlusame}

Oui, vous pouvez utiliser le même IBMid pour vous connecter à l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} et à {{site.data.keyword.Bluemix_notm}}.


## J'ai lié un compte {{site.data.keyword.Bluemix_notm}}, comment dois-je faire pour donner accès aux membres d'équipe de mon autre infrastructure {{site.data.keyword.BluSoftlayer_notm}} ?
{: #bicp_linkgiveteamaccess}

Vous devez les inviter à {{site.data.keyword.Bluemix_notm}}. Dans l'interface utilisateur de {{site.data.keyword.Bluemix_notm}}, sélectionnez **Compte et support** > **Compte** > **Inviter des membres d'équipe**. Après avoir sélectionné un groupe de ressources, vous verrez une option permettant d'ajouter des membres d'équipe de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Vous devrez peut-être vous connecter à l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour pouvoir envoyer des invitations. {{site.data.keyword.Bluemix_notm}} extrait la liste des utilisateurs de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}, puis vous pouvez sélectionner ceux que vous souhaitez inviter pour le compte {{site.data.keyword.Bluemix_notm}}.


## Où se trouve mon e-mail pour effectuer le passage à IBMid ?
{: #bicp_ibmidswitchemail}

Si vous avez suivi l'assistant pour passer à IBMid et n'avez pas reçu l'e-mail, sachez que l'envoi du courrier contenant votre code d'enregistrement peut prendre de quelques minutes à plusieurs heures. Vous pouvez revenir à la page **Modifier profil utilisateur** du portail client et cliquer sur **Renvoyer l'e-mail** pour renouveler l'opération.


## Est-ce que je disposerai de droits d'accès de l'utilisateur root complets à mon compte ?
{: #bicp_fullrootaccaccess}

Les utilisateurs principaux et les utilisateurs dotés de droits d'administrateur possèdent des droits d'accès root complets sur le portail client et l'API. L'accessibilité des utilisateurs dotés de droits d'administrateur est contrôlée par les utilisateurs ayant un rôle administratif. Ces droits peuvent être mis à jour à tout moment en [éditant le profil utilisateur](edit-user-profile.html) sur le portail client.


## Puis-je lier un compte d'abonnement {{site.data.keyword.Bluemix_notm}} ?
{: #bicp_linkbmxsubacct}

Tous les comptes liés dans {{site.data.keyword.Bluemix_notm}} doivent être des comptes de type Paiement à la carte. Vous pouvez créer un compte de paiement à la carte ou lier un compte existant. Ou bien, vous pouvez lier un compte d'essai existant, mais celui-ci sera mis à niveau vers un compte de paiement à la carte.


## Comment supprimer le lien de mon compte {{site.data.keyword.Bluemix_notm}} avec mon compte d'infrastructure {{site.data.keyword.BluSoftlayer_notm}} ?
{: #bicp_unlinkacct}

Une fois que des comptes sont liés, cette opération est irréversible.


## Qu'est-ce que mon profil de société et où puis-je le trouver ?
{: #bicp_whatfindcompprof}

Le profil de société correspond aux informations soumises lors de la création du compte et inclut un contact principal pour votre société, ainsi que le nom, l'adresse et le numéro de téléphone de la société. Ces informations sont utilisées pour différentes raisons et doivent être conservées à jour en permanence. Pour afficher le profil de société de votre compte ou demander des modifications, voir [Mise à jour de votre profil de société](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch).

## Où se trouvent les mots de passe de mon appareil et du logiciel ?
{: #bicp_devswpw}

Les mots de passe d'appareil et de logiciel sont stockés à deux emplacements sur le [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Pour extraire les donnée d'identification de l'appareil, y compris le nom d'utilisateur root ou administrateur et les mots de passe pour {{site.data.keyword.baremetal_short}} et {{site.data.keyword.virtualmachinesshort}}, voir la rubrique sur l'[interaction avec un appareil dans la vue Instantané](/docs/vsi/vsi_interact_device_snapshot_view.html). Pour rapidement afficher et extraire les données d'identification du logiciel qui sont manuellement suivies via le portail client, voir la rubrique sur la [gestion des accès à l'équipement](/docs/vsi/vsi_device_access.html).

##Comment garder mes données Web synchronisées ?
{: #bicp_webdatasync}

Bien que vous soyez responsable de la conservation de la cohérence des données entre les serveurs réels, {{site.data.keyword.BluSoftlayer_full}} fournit un réseau privé que vous pouvez utiliser pour la synchronisation sans frais d'utilisation.


## Qu'est-ce que le système de gestion d'événements ?
{: #bicp_whatisems}

Le système de gestion d'événements est un outil qui optimise la façon dont {{site.data.keyword.BluSoftlayer_full}} partage avec les utilisateurs des informations sur les problèmes d'infrastructure imprévus et les événements de maintenance planifiée à venir. Il utilise des alertes e-mail ciblées, basées sur un abonnement, pour ces incidents afin de partager le type d'événement survenu. Il fournit aux utilisateurs abonnés des détails supplémentaires sur l'impact global de l'événement, ainsi qu'un statut en cours de l'incident imprévu en cours (UIP).

## Comment et où puis-je annuler un équipement ?
{: #bicp_candev}

Vous pouvez à tout moment annuler un appareil via le [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Voir la rubrique relative à l'[annulation d'appareil](/vsi/vsi_managing.html) pour plus d'informations sur l'exécution d'une demande d’annulation.
