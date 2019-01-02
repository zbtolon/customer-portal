---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Ajout d'utilisateurs à un compte SoftLayer
{: #customerportal_addusertocpacct}

Un ou plusieurs utilisateurs peuvent interagir avec les produits et services associés à un compte. Si vous êtes l'utilisateur principal ou si vous avez un accès administrateur, vous pouvez ajouter des utilisateurs. {:shortdesc}

Si vous gérez des utilisateurs de l'infrastructure {{site.data.keyword.BluSoftlayer_full}}, les comptes SoftLayer que vous pouvez gérer dépendent de l'accès affecté à votre compte utilisateur. Ils dépendent également de la façon dont votre compte a été configuré. Si vous êtes l'utilisateur principal, ou si vous disposez d'un accès administrateur en tant que propriétaire de compte, vous pouvez gérer d'autres utilisateurs du portail client. Si votre compte n'est pas configuré en tant qu'utilisateur principal, vous pouvez gérer votre profil utilisateur.

En fonction de votre accès, vous pouvez gérer votre compte SoftLayer ou les comptes d'autres utilisateurs depuis la fenêtre Utilisateurs. La fenêtre Utilisateurs dans le [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} affiche les utilisateurs associés à un compte. Les interactions disponibles dans la fenêtre Utilisateurs varient en fonction de l'ensemble de vos droits de compte uniques.
  * Si vous êtes l'utilisateur principal du compte, vous pouvez voir tous les utilisateurs associés au compte.

  Si vous devez partager les identifiants de connexion principaux de votre compte, faites-le avec prudence. Votre connexion principale contrôle chaque aspect de votre compte et vous devez la protéger. Pour permettre à d'autres utilisateurs de se servir du portail client, vous configurez des utilisateurs individuels ou basés sur des permissions. La création d'utilisateurs sur la base de permissions vous permet de contrôler étroitement quels utilisateurs sont habilités à interagir avec certains aspects de votre compte.
{:tip}

  * Si vous disposez d'un accès administrateur, vous pouvez voir tous les utilisateurs que vous avez ajoutés. Si vous les avez autorisés à gérer d'autres utilisateurs, vous pouvez voir tous les utilisateurs qu'ils ont ajoutés. Vous pouvez également gérer tout utilisateur associé au compte. Vous pouvez aussi éditer l'accès au portail client, changer le statut utilisateur et retirer des utilisateurs.

Pour gérer des utilisateurs depuis la console {{site.data.keyword.Bluemix_notm}}, voir [Gestion de votre compte](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) et [Gestion de l'identité et de l'accès](/docs/iam/quickstart.html#getstarted). Pour plus d'informations sur la console {{site.data.keyword.Bluemix_notm}}, voir la section [Navigation dans la console {{site.data.keyword.Bluemix_notm}}](/docs/overview/ui.html#ui).

Différentes personnes au sein d'une organisation possèdent différents rôles et responsabilités, et les ensembles de droits utilisateur ne sont pas identiques pour tous. Vous pouvez ajouter au portail client des utilisateurs dotés de rôles leur permettant un accès uniquement à ce que requiert leur rôle spécifique. Si des changements sont faits par erreur ou n'ont pas été autorisés, vous pouvez les tracer jusqu'à l'utilisateur ou le groupe. Vous pouvez donc leur fournir une formation adéquate ou mettre à jour les droits utilisateur afin de minimiser les risques. Vos utilisateurs peuvent alors se concentrer sur leur rôle spécifié dans le portail client.

Utilisez la procédure suivante pour ajouter un utilisateur à un compte :

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur **Ajouter un utilisateur**.
4. Renseignez les champs obligatoires dans la section **Informations personnelles**. Indiquez un statut, un nom d'utilisateur et l'adresse de courrier électronique pour la communication sur le portail client et les notifications, y compris la notification initiale afin de configurer un mot de passe pour le compte.

  Plutôt que d'entrer une adresse pour l'utilisateur, vous avez la possibilité de cocher la case **Utiliser les informations par défaut de l'entreprise** pour renseigner l'adresse de la société.
  {: tip}

5. Renseignez les champs obligatoires dans la section **Paramètres de connexion**. Indiquez si les paramètres peuvent être modifiés par l'utilisateur, si l'adresse IP est restreinte et si l'utilisateur est requis de configurer et d'utiliser des questions de sécurité. En outre, pour les personnes n'utilisant pas d'IBMid, vous pouvez définir la durée avant expiration du mot de passe.
**Remarques :**
* Si vous utiliser IBMid pour l'authentification mettez à jour les mots de passe dans vos [profils IBMid ![Icône de lien externe](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} en suivant les instructions sous l'**ouverture de session**.
* Cochez la case **Utiliser le mot de passe du portail pour le VPN** pour synchroniser les mots de passe du portail client et du réseau privé virtuel.
6. Cliquez sur **Ajouter un utilisateur**.

Après que vous avez créé un compte pour l'utilisateur, ce dernier reçoit une notification par courrier électronique l'avisant de compléter la configuration de son compte. L'utilisateur doit configurer un mot de passe et éventuellement créer des questions de sécurité si vous avez indiqué qu'elles sont obligatoires.

La façon dont les utilisateurs sans l'accès administrateur d'un utilisateur principal se connectent au portail client dépend de l'utilisateur principal qui a fourni l'accès utilisateur dans leurs comptes SoftLayer :
  * Si l'utilisateur principal utilise un IBMid pour s'authentifier, chaque utilisateur qu'il crée possède un IBMid.
  * Si l'utilisateur principal utilise un ID d'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour l'authentification, chaque utilisateur qu'il crée possède un nom d'utilisateur de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. L'utilisateur principal de chaque utilisateur créé doit exécuter l'outil de migration pour passer à un IBMid.
  * Si aucun de ces cas ne s'applique, pour des partenaires commerciaux IBM par exemple, contactez le support afin de déterminer l'ID utilisateur à utiliser.

## Définition des droits utilisateurs sur le compte
{: #cp_setuserpermsacct}

Utilisez la procédure suivante pour définir les droits de l'utilisateur que vous venez d'ajouter.

1. Cliquez sur l'icône **Autorisations**, qui représente une silhouette d'utilisateur avec un verrou.
2. Mettez à jour les **autorisations utilisateur** dans tous les onglets du nouvel utilisateur.
> **Remarque :** Sélectionnez une option dans la liste **Droits rapides** pour afficher les ensembles de droits pour trois types d'utilisateur. Cliquez sur **Définir droits** pour sélectionner l'ensemble de droits ou personnalisez l'accessibilité de l'utilisateur en sélectionnant des options individuelles sur chaque onglet disponible.
3. Cliquez sur **Ajouter droits pour le portail** pour ajouter les droits ou cliquez sur **Réinitialiser droits** pour réinitialiser les droits de l'utilisateur.
4. Cliquez sur l'icône **Accès à l'Unité**, qui représente trois serveurs.
5. Cochez la case de chaque unité à laquelle vous souhaitez que l'utilisateur puisse accéder.
6. Cliquez sur **Mettre à jour l'accès à l'unité** une fois les unités sélectionnées.

Vous recevrez un e-mail avec des liens et des informations pour vous guider dans la configuration d'un IBMid pour l'authentification pour ce compte. Les étapes peuvent inclure la création d'un nouvel IBMid si le compte utilise IBMid pour l'authentification. L'invitation expire sous 7 jours, mais vous pouvez contacter votre administrateur pour qu'il renvoie l'invitation.

Pour tous les autres cas d'authentification, une fois le nouvel utilisateur ajouté, il peut se connecter n'importe quand au portail client. Les utilisateurs peuvent utiliser les divers produits et services associés au compte. Vous pouvez désactiver l'utilisateur à tout moment.
