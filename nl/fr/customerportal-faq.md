---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-16"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Foire aux questions
{: #bicpfaq}

## Comment extraire mes données d'identification pour le portail client ?
{: #bicp_retcreds}

Si vous utilisez votre IBMid pour l'authentification, lorsque vous passez votre première commande ou que vous êtes ajouté en tant qu'utilisateur dans un compte, vous recevez un e-mail comportant un lien pour vous permettre de débuter avec votre IBMid. Si vous perdez ou oubliez votre nom d'utilisateur ou votre mot de passe, accédez à votre [profil IBMid![External link icon](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} et réinitialisez ou récupérez le mot de passe en suivant les instructions fournies après le processus de connexion. Vous serez invité à entrer des informations spécifiques, lesquelles peuvent inclure des réponses à vos questions de sécurité.

Si vous n'utilisez pas d'IBMid pour l'authentification, lorsque vous passez votre première commande ou que vous êtes ajouté en tant qu'utilisateur d'un compte dans le [portail client![External link icon](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, vous recevez un e-mail contenant votre nom d'utilisateur et votre mot de passe initial pour débuter sur le portail client. Prenez soin de changer votre mot de passe après vous être connecté pour la première fois en éditant votre profil utilisateur. 

Si vous oubliez votre mot de passe après votre connexion, utilisez la fonction **Mot de passe oublié** disponible sur l'écran de connexion du portail client. Vous serez invité à entrer des informations spécifiques, et notamment à répondre à un ensemble de questions de sécurité que vous avez spécifiées lors de la configuration de votre profil utilisateur.

Si vous oubliez votre nom d'utilisateur, contactez votre administrateur de compte ou utilisateur principal, qui dispose des droits pour extraire votre nom d'utilisateur. Si vous êtes l'administrateur ou l'utilisateur principal sur le compte, contactez le support pour une aide supplémentaire.

## Qu'est-ce que l'IBMid ?
{: #bicp_whatisibmid}

Les nouveaux comptes nécessitent un IBMid pour l'authentification. Les comptes existants continuent d'utiliser les nom d'utilisateur et mot de passe SoftLayer pour l'authentification tant que vous n'avez pas exécuté l'outil de migration pour passer à un IBMid. Votre compte SoftLayer possède un utilisateur principal doté des droits d'ajout d'autres utilisateurs au sein de ce même compte. Voir [Gestion des comptes SoftLayer dans le portail client](/docs/customer-portal/cphowacctsman.html) pour plus d'informations.

## Comment lier un compte SoftLayer existant ?
{: #bicp_linkbmxacct}

Si vous êtes l'utilisateur principal sur votre compte SoftLayer, connectez-vous au portail client et cliquez sur **Lier le compte** dans l'en-tête.  Voir [Liaison de comptes utilisateur IBMid](/docs/account/softlayerlink.html) pour plus d'informations.

## Faut-il être un utilisateur {{site.data.keyword.Bluemix_notm}} existant pour lier des comptes ?
{: #bicp_bmxusertolink}

Non. Vous pouvez créer un compte {{site.data.keyword.Bluemix_notm}} ou lier un compte {{site.data.keyword.Bluemix_notm}} existant de type Lite ou Paiement à la carte.

## Comment l'authentification à deux facteurs opère-t-elle ?
{: #bicp_2fa}

La configuration d'une authentification à deux facteurs (2FA) n'a pas d'impact au niveau du compte. L'authentification 2FA n'opère pas au niveau de l'IBMid, mais per compte. Quand un IBMid est associé à plusieurs comptes et que vous basculez d'un compte à l'autre, vous devez confirmer votre identité chaque fois que vous passez à un compte différent qui nécessite une authentification 2FA. Cette règle s'applique même si le compte précédent et le nouveau compte sont tous les deux configurés avec le même mécanisme d'authentification 2FA.

Pour plus d'informations sur l'IBMid avec authentification 2FA, voir [Utilisation de l'authentification à deux facteurs dans les comptes liés](/docs/account/softlayerlink.html).

## Qui peut lier des comptes ?
{: #bicp_wholinkaccts}

Seuls les utilisateurs principaux de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} peuvent lier des comptes SoftLayer et {{site.data.keyword.Bluemix_notm}}. L'e-mail d'un utilisateur principal doit également être associé au propriétaire principal du compte {{site.data.keyword.Bluemix_notm}} à lier.

## Que dois-je utiliser pour me connecter à chaque console ?
{: #bicp_logineachport}

La facturation de vos comptes est liée et vous pouvez aisément passer de votre compte SoftLayer à votre compte {{site.data.keyword.Bluemix_notm}} et vice-versa, mais les identités de vos comptes restent distinctes.

* Si votre compte n'utilise pas IBMid pour l'authentification, continuez à utiliser votre ID SoftLayer pour les produits et services SoftLayer et utilisez votre IBMid pour les produits et services {{site.data.keyword.Bluemix_notm}}.

* Si votre compte utilise IBMid pour l'authentification, vous utilisez votre IBMid pour accéder à vos comptes SoftLayer et {{site.data.keyword.Bluemix_notm}}.

## Pourquoi une erreur est-elle renvoyée lorsque je tente de me connecter avec mon nom d'utilisateur SoftLayer ?
{: #bicp_SLloginerror}

Une fois que vous êtes passé à un IBMid, si vous vous connectez au portail client avec votre nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}, une erreur "Données d'identification incorrectes" est affichée. Une fois passé à un IBMid, vous ne pouvez plus vous connecter au portail client avec votre nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Vous devez cliquer sur **Connexion avec identité IBM** dans la boîte de dialogue Connexion au Compte.

## Pourquoi une erreur est-elle renvoyée lorsque je tente de me connecter avec mon IBMid ?
{: #bicp_IBMidloginerror}

Lorsque vous vous connectez avec votre IBMid, l'erreur "Nous ne reconnaissons pas cet IBMid ou cette adresse électronique." s'affiche. Prenez soin d'entrer une adresse électronique qualifiée complète. Vérifiez également que vous n'utilisez pas votre nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.

## Les membres de l'équipe d'infrastructure {{site.data.keyword.BluSoftlayer_notm}} peuvent-ils accéder à mon compte lié ?
{: #bicp_linkgiveteamaccess}

Vous devez les inviter à {{site.data.keyword.Bluemix_notm}}. Dans la console {{site.data.keyword.Bluemix_notm}}, cliquez sur **Gérer** > **Compte** > **Utilisateurs**. Après avoir sélectionné un groupe de ressources, vous pouvez ajouter des membres de l'équipe d'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Vous devrez éventuellement vous connecter au portail client avant de pouvoir envoyer des invitations. {{site.data.keyword.Bluemix_notm}} extrait la liste des utilisateurs de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}, puis vous pouvez sélectionner ceux que vous souhaitez inviter pour le compte {{site.data.keyword.Bluemix_notm}}.

## Où se trouve mon e-mail pour effectuer le passage à IBMid ?
{: #bicp_ibmidswitchemail}

Si vous avez suivi l'assistant pour passer à IBMid et n'avez pas reçu l'e-mail, sachez que l'envoi du courrier contenant votre code d'enregistrement peut prendre de quelques minutes à plusieurs heures. Pour effectuer une nouvelle tentative, vous pouvez revenir à la page **Modifier profil utilisateur** et cliquer sur **Renvoyer le courrier électronique**.

## Disposerai-je de droits d'accès complets de l'utilisateur root sur mon compte ?
{: #bicp_fullrootaccaccess}

Les utilisateurs principaux et les utilisateurs dotés de droits d'administrateur possèdent des droits d'accès root complets sur le portail client et l'API. L'accessibilité des utilisateurs dotés de droits d'administrateur est contrôlée par les utilisateurs ayant un rôle administratif. Ces droits peuvent être mis à jour par des administrateurs à partir du portail client en [éditant un profil utilisateur](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Si vous ne disposez pas de droits d'administrateur, vous pouvez éditer votre profil utilisateur dans le portail client en cliquant sur votre nom d'utilisateur dans le panneau supérieur.

## Puis-je lier un compte {{site.data.keyword.Bluemix_notm}} de type Abonnement ?
{: #bicp_linkbmxsubacct}

Tous les comptes liés dans {{site.data.keyword.Bluemix_notm}} doivent être du type Lite ou Paiement à la carte. 

## Comment supprimer le lien de mon compte ?
{: #bicp_unlinkacct}

Une fois que des comptes sont liés, cette opération est irréversible.


## Qu'est-ce que mon profil de société et où puis-je le trouver ?
{: #bicp_whatfindcompprof}

Le profil de société correspond aux informations soumises lors de la création du compte et inclut un contact principal pour votre société, ainsi que le nom de la société, son adresse et son numéro de téléphone. Ces informations sont utilisées pour différentes raisons et doivent être conservées à jour en permanence. Pour afficher le profil de société de votre compte ou demander des modifications, voir [Mise à jour de votre profil de société](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch).

## Où se trouvent les mots de passe de mon appareil et du logiciel ?
{: #bicp_devswpw}

Les mots de passe du périphérique et du logiciel sont stockés à deux emplacements dans le portail client. Pour extraire les donnée d'identification de l'appareil, y compris le nom d'utilisateur root ou administrateur et les mots de passe pour {{site.data.keyword.baremetal_short}} et {{site.data.keyword.virtualmachinesshort}}, voir la rubrique sur l'[interaction avec un appareil dans la vue Instantané](/docs/vsi/vsi_interact_device_snapshot_view.html).  Pour examiner et extraire rapidement les données d'identification auprès du logiciel suivies manuellement via le portail client, voir [Gestion des accès à l'équipement](/docs/vsi/vsi_device_access.html).

## Comment garder mes données Web synchronisées ?
{: #bicp_webdatasync}

Bien que vous soyez responsable du maintien de la cohérence des données entre les serveurs réels, {{site.data.keyword.BluSoftlayer_full}} fournit un réseau privé que vous pouvez utiliser pour synchronisation sans encourir de frais d'utilisation.

## Qu'est-ce que le système de gestion d'événements ?
{: #bicp_whatisems}

Le système de gestion d'événements est un outil qui optimise la façon dont {{site.data.keyword.BluSoftlayer_full}} partage avec les utilisateurs des informations sur les problèmes d'infrastructure imprévus et les événements de maintenance planifiée à venir. Il utilise des alertes e-mail ciblées, basées sur un abonnement, pour ces incidents afin de partager le type d'événement survenu. Il fournit aux utilisateurs abonnés des détails supplémentaires sur l'impact global de l'événement, ainsi qu'un statut en cours de l'incident imprévu en cours (UIP).

## Puis-je annuler un appareil ?
{: #bicp_candev}

Vous pouvez à tout moment annuler un appareil via le portail client. Voir la rubrique relative à l'[annulation d'appareil](/docs/vsi/vsi_managing.html) pour plus d'informations sur l'exécution d'une demande d’annulation.
