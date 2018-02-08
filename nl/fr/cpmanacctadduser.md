---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-05"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Ajout d'utilisateurs à un compte SoftLayer
{: #customerportal_addusertocpacct}

Un ou plusieurs utilisateurs peuvent interagir avec les produits et services associés à un compte. Si vous êtes l'utilisateur principal, vous pouvez ajouter des utilisateurs à tout moment.
{:shortdesc}

Si vous gérez des utilisateurs de l'infrastructure {{site.data.keyword.BluSoftlayer_full}}, les comptes SoftLayer que vous pouvez gérer dépendent de l'accès affecté à votre compte utilisateur et de la façon dont votre compte a été configuré. Si vous êtes l'utilisateur principal, ou si vous disposez d'un accès administrateur en tant que propriétaire de compte, vous pouvez gérer d'autres utilisateurs du portail client. Si votre compte n'est pas configuré en tant qu'utilisateur principal, vous pouvez gérer votre profil utilisateur.

En fonction de votre accès, vous pouvez gérer votre compte SoftLayer ou les comptes d'autres utilisateurs depuis la fenêtre Utilisateurs. Cette fenêtre du [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} affiche les utilisateurs associés à un compte. Les interactions disponibles dans la fenêtre Utilisateurs varient en fonction de l'ensemble de vos droits de compte uniques. 
  * Si vous êtes l'utilisateur principal du compte, vous pouvez voir tous les utilisateurs associés au compte. 

  Si vous devez partager les identifiants de connexion principaux de votre compte, faites-le avec prudence. Votre connexion principale contrôle chaque aspect de votre compte et doit être protégée. Pour permettre à d'autres utilisateurs de se servir du portail client, vous configurez des utilisateurs individuels ou basés sur des permissions. Vous disposez ainsi d'un contrôle maximal sur les personnes pouvant interagir avec certains aspects de votre compte.
  {:tip}
  * Si vous disposez d'un accès administrateur, vous pouvez voir tous les utilisateurs que vous avez créés et, si vous leur avez donné le droit d'administrer d'autres utilisateurs, vous pouvez également voir les utilisateurs qu'ils ont créés. Vous pouvez également exécuter des actions sur tout utilisateur associé au compte, y compris éditer l'accès au portail client, changer le statut utilisateur ou retirer des utilisateurs.
  * Si vous n'êtes pas l'utilisateur principal du compte, et si vous ne disposez pas d'un accès administrateur, seul votre profil s'affiche. Vous pouvez interagir avec votre propre compte, notamment en affichant la clé d'API, en éditant l'accès au VPN ou en ajoutant une authentification externe. 

Pour gérer des utilisateurs depuis la console {{site.data.keyword.Bluemix_notm}}, voir [Gestion de votre compte](/docs/admin/adminpublic.html#signing-up-for-ibm-cloud) et [Gestion de l'identité et de l'accès](/docs/iam/quickstart.html#getstarted). Voir [Fonctionnement de la console {{site.data.keyword.Bluemix_notm}}](/docs/overview/ui.html#ui) pour plus d'informations sur la console {{site.data.keyword.Bluemix_notm}}.

Différentes personnes au sein d'une organisations possèdent différents rôles et responsabilités, et les ensembles de droits utilisateur ne sont pas identiques pour tous. C'est pourquoi vous pouvez ajouter des utilisateurs au portail client avec des rôles garantissant que chaque personne ou groupe accède uniquement aux éléments qu'il doit. Si des changements sont faits par erreur ou n'ont pas été autorisés, vous pouvez les tracer jusqu'à l'utilisateur ou le groupe afin d'être sûr de fournir une formation appropriée ou de mettre à jour les droits utilisateurs. Cela limite le risque de différentes façons et permet aux utilisateurs de se concentrer sur leur rôle spécifique sur le portail client. 

Utilisez la procédure suivante pour ajouter un utilisateur à un compte :

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur **Ajouter un utilisateur**.
4. Renseignez les zones requises de la section **Informations personnelles**, notamment le statut, un nom d'utilisateur et l'adresse e-mail pour la communication sur le portail client et les notifications, y compris la notification initiale de configuration d'un mot de passe pour le compte.

  Plutôt que d'entrer une adresse pour l'utilisateur, vous avez la possibilité de cocher la case **Utiliser les informations par défaut de l'entreprise** pour renseigner l'adresse de la société.
  {: tip}

5. Renseignez les zones requises à la section **Paramètres de connexion**, notamment en indiquant si les paramètres peuvent ou non être édités par l'utilisateur, si l'adresse IP est restreinte, et si l'utilisateur doit ou non configurer et utiliser des questions de sécurité. En outre, pour les personnes n'utilisant pas d'IBMid, vous pouvez définir la durée avant expiration du mot de passe.
**Remarques :**
* Si vous utiliser IBMid pour l'authentification mettez à jour les mots de passe dans vos [profils IBMid ![Icône de lien externe](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} en suivant les instructions sous l'**ouverture de session**.
* Cochez la case du **mot de passe de l'utilisateur du portail pour VPN** pour synchroniser les mots de passe VPN et du portail client. 
6. Cliquez sur **Ajouter un utilisateur**.

Après que vous avez créé un compte pour un utilisateur, l'utilisateur reçoit une notification par e-mail pour terminer la configuration de son compte en définissant un mot de passe et, éventuellement des questions de sécurité si vous avez indiqué qu'elles étaient obligatoires.

La façon dont les utilisateurs sans l'accès administrateur d'un utilisateur principal se connectent au portail client dépend de l'utilisateur principal qui a fourni l'accès utilisateur dans leurs comptes SoftLayer.
  * Si l'utilisateur principal utilise un IBMid pour s'authentifier, chaque utilisateur qu'il crée possède un IBMid.
  * Si l'utilisateur principal utilise un ID d'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour l'authentification, chaque utilisateur qu'il crée possède un nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. L'utilisateur principal de chaque utilisateur créé doit exécuter l'outil de migration pour passer à un IBMid.
  * Si aucun de ces cas ne s'applique, pour des partenaires commerciaux IBM par exemple, contactez le support afin de déterminer l'ID utilisateur à utiliser.

## Définition des droits utilisateurs sur le compte
{: #cp_setuserpermsacct}

Utilisez la procédure suivante pour définir les droits de l'utilisateur que vous venez d'ajouter.

1. Cliquez sur l'icône **Autorisations**, qui représente une silhouette d'utilisateur avec un verrou.
2. Mettez à jour les **autorisations utilisateur** dans tous les onglets du nouvel utilisateur.
> **Remarque :** Sélectionnez une option dans la liste **Droits rapides** pour afficher les ensembles de droits recommandés pour trois types d'utilisateur. Cliquez sur **Définir droits** pour sélectionner l'ensemble recommandé, ou personnalisez l'accessibilité de l'utilisateur en sélectionnant des options individuelles sur chaque onglet disponible. 
3. Cliquez sur **Ajouter droits pour le portail** pour ajouter les droits ou cliquez sur **Réinitialiser droits** pour réinitialiser les droits de l'utilisateur. 
4. Cliquez sur l'icône **Accès à l'Unité**, qui représente trois serveurs.
5. Cochez la case de chaque unité à laquelle vous souhaitez que l'utilisateur puisse accéder. 
6. Cliquez sur **Mettre à jour l'accès à l'unité** une fois les unités sélectionnées. 

Vous recevrez un e-mail avec des liens et des informations pour vous guider dans la configuration d'un IBMid pour l'authentification pour ce compte. Les étapes peuvent inclure la création d'un nouvel IBMid si le compte utilise IBMid pour l'authentification. L'invitation expire sous 7 jours, mais vous pouvez contacter votre administrateur pour qu'il renvoie l'invitation.

Pour tous les autres cas d'authentification, une fois le nouvel utilisateur ajouté, il peut se connecter à tout moment au portail client pour utiliser différents produits et services associés au compte. Vous pouvez désactiver l'utilisateur à tout moment.
