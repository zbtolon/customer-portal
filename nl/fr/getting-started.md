---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-15"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Tutoriel d'initiation
{: #getting-started}

Dans ce tutoriel, nous allons détailler la procédure pour vous rendre opérationnel avec votre compte SoftLayer afin que vous puissiez commencer à passer des commandes et gérer vos ressources d'infrastructure.
{:shortdesc}

## Avant de commencer
{: #prereqs}

Vous aurez besoin d'un compte [{{site.data.keyword.Bluemix}} ![Icône de lien externe](../icons/launch-glyph.svg "Icône de lien externe")](https://control.bluemix.net/){:new_window}. Connectez-vous au portail client à l'aide de vos données d'identification IBMid. La plupart des nouveaux utilisateurs se servent de l'[IBMid](/docs/account/softlayerlink.html#switchtoIBMid) pour l'authentification.

Si vous n'employez pas d'IBMid pour l'authentification afin de vous connecter à votre compte, connectez-vous au portail client avec vos données d'identification uniques de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.
{: tip}

## Etape 1 : Configurer votre compte
{: #account-setup}

La configuration de votre compte inclut la vérification de vos informations de contact et des détails de facturation :
 * Pour vérifier les détails de contact de votre entreprise, accédez à **Compte** > **Gérer** > **Contacts de la société**. Les informations de contact de l'entreprise de votre compte sont utilisées pour vous notifier des éventuels problèmes ou des modifications apportées à votre compte.
 * Pour vérifier les détails de votre profil de société, accédez à **Compte** > **Gérer** > **Profil de la Société**. Les informations de profil de l'entreprise contiennent des détails relatifs au titulaire de compte principal.
 * Pour vérifier vos détails de facturation, accédez à **Compte** > **Facturation** > **Mode de Règlement**. Le mode de règlement mensuel repose sur la carte de crédit facturée sur une base récurrente pour les paiements associés à votre compte.

## Etape 2 : Ajouter des utilisateurs et affecter des droits
{: #users-permissions}

Pour ajouter des utilisateurs à votre compte et définir les droits initiaux, accédez à **Compte** > **Utilisateurs**.
 * Pour inviter des utilisateurs à accéder aux ressources de plateforme et d'infrastructure de votre compte en fonction des droits spécifiques que vous avez affectés, cliquez sur **Inviter des utilisateurs**. Vous êtes ensuite dirigé vers l'interface utilisateur {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) pour inviter les utilisateurs et affecter les accès. Voir [Invitation d'utilisateurs et affectation d'accès](/docs/iam/iamuserinv.html) pour plus d'informations.
 * Pour ajouter des utilisateurs avec un accès VPN uniquement, cliquez sur l'option d'**ajout d'utilisateur VPN uniquement**. Entrez les informations personnelles, définissez les droits d'accès au portail et définissez l'accès aux unités pour l'utilisateur.

Lorsque vous définissez des droits d'accès à l'infrastructure dans l'invitation initiale, vous choisissez parmi l'un des trois ensembles de droits : Affichage uniquement, Utilisateur de base, Superutilisateur. Une fois que l'utilisateur a accepté l'invitation, vous pouvez personnaliser son accès en éditant les droits d'accès au portail. Pour plus d'informations, voir [Droits relatifs à l'infrastructure](/docs/iam/infrastructureaccess.html).
{: tip}

## Etape 3 : Activer l'accès au réseau privé de l'infrastructure {{site.data.keyword.Bluemix_notm}}
{: #enable-private-network}

Le réseau privé de l'infrastructure {{site.data.keyword.Bluemix_notm}} est proposée gratuitement aux utilisateurs et appareils. Toute la bande passante utilisée sur le réseau privé est illimitée et gratuite. Le réseau privé offre de nombreux avantages, notamment :
  * La réplication d'environnements d'unités vers d'autres centres de données pour la reprise en ligne
  * L'accessibilité du système frontal aux serveurs de base de données
  * L'accès sécurisé et la gestion de vos systèmes

Pour activer l'accès utilisateur au réseau privé, éditez l'accès VPN sur le portail client :
  1. Sélectionnez **Compte** > **Accès VPN** dans la barre de menus.  
  2. Cliquez sur le lien dans la colonne Accès VPN.
  3. Sélectionnez une option dans le menu **Type de VPN** et cliquez sur **Enregistrer**.  

Pour les utilisateurs de comptes utilisant l'authentification IBMid, le nom d'utilisateur VPN SoftLayer pour l'accès VPN est utilisé. Le nom d'utilisateur VPN est défini dans le profil utilisateur. Le nom d'utilisateur VPN est différent du nom d'utilisateur dont la valeur par défaut est l'adresse e-mail et l'ID de compte IBMid.
{: tip}

Pour plus d'informations sur l'utilisation d'une connexion VPN, voir [A propos de la connexion VPN](/docs/infrastructure/iaas-vpn/about-vpn.html).

## Etape 4 : S'abonner aux notifications
{: #get-notified}

Pour être notifié des problèmes système pouvant survenir ainsi que des événements de maintenance planifiée, vous pouvez vous abonner aux notifications via le système de gestion d'événements. Lorsque vous créez un compte ou que vous êtes ajouté à un compte, vous êtes par défaut désabonné des notifications.

Accédez au système de gestion d'événements sur le portail client pour choisir le type des notifications auxquelles vous souhaitez vous abonner :
  1. Sélectionnez **Compte** > **Gérer** > **Abonnements** dans la barre de menus.
  2. Cliquez sur un abonnement spécifique dans la liste.
  3. Cochez la case **Oui** dans la colonne Abonné.
  4. Cliquez sur **Afficher Tous les Abonnements** pour revenir à la liste des abonnements disponibles et abonnez-vous à d'autres types si nécessaire.

## Etapes suivantes
{: #next-steps}

Une fois votre compte configuré, accédez au [catalogue {{site.data.keyword.Bluemix_notm}} ![Icône de lien externe](../icons/launch-glyph.svg)](https://console.bluemix.net/catalog/?category=infrastructure){:new_window} et commencez à commander des équipements.
