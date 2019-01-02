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


# Gestion d'un profil utilisateur
{: #customerportal_accuserprof}

Sur le portail client, un profil utilisateur inclut différentes données sur l'utilisateur, notamment les informations de contact et la clé d'API. C'est également là que sont stockés les mots de passe. Si vous disposez d'un accès administrateur, vous pouvez changer les droits et l'accès à l'unité depuis le profil.
{:shortdesc}

Dans le profil utilisateur, vous pouvez gérer les informations de contact et les mots de passe, afficher les clés d'API et mettre à jour les droits et l'accès à l'unité en fonction de vos droits.

## Edition d'un profil utilisateur
{: #cp_edituserprofile}

Après qu'un profil utilisateur ait été créé sur le portail client, vous pouvez l'éditer à tout moment. Les détails associés au profil utilisateur incluent les informations personnelles, les paramètres de connexion, les détails d'accès aux API, les abonnements aux notifications utilisateur, ainsi que les questions de sécurité. Utilisez la procédure suivante pour éditer un profil utilisateur.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur le nom d'utilisateur pour accéder au profil utilisateur associé pour cet utilisateur.
4. Editez les détails du **Profil utilisateur** selon les besoins. Pour les utilisateurs de comptes utilisant IBMid pour l'authentification, mettez à jour vos adresse e-mail et mot de passe dans votre profil IBMid. Voir le tableau 1 pour plus d'informations. 
5. Si vous désirez réinitialiser votre mot de passe après vous être connecté, cliquez sur **Réinitialiser le mot de passe** afin de générer un courrier électronique qui vous permet de changer votre mot de passe.
6. Cliquez sur **Editer l'utilisateur** pour soumettre les modifications.

| Zone | Définition |
|-----|----------|
| Prénom, Nom | Prénom et nom de l'utilisateur associé au profil utilisateur.|
| Adresse e-mail | Adresse e-mail préférée pour réception de notifications de l'infrastructure  {{site.data.keyword.BluSoftlayer_notm}} sur le compte. La modification de l'adresse e-mail change l'enregistrement dans l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Ce changement n'affecte pas la liaison vers les données d'authentification IBMid. Vous devez modifier l'adresse e-mail pour l'IBMid depuis le profil IBMid.|
| Fuseau horaire | Fuseau horaire à utiliser de préférence lors de l'affichage des données horodatées.|
| Téléphone, Autre téléphone| Numéros de téléphone préférés à utiliser par l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.|
| Rue, Ville, Pays, Etat/Province, Code postal | Adresse complète du contact, à utiliser par l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.|
{: caption="Tableau 1. Paramètres de configuration des informations personnelles pour l'édition d'un profil utilisateur" caption-side="top"}

|Zone|Définition|
|-----|----------|
| Limiter l'accès à l'adresse IP | Adresse IP à laquelle restreindre l'accès lorsque vous tentez d'utiliser le portail client sous le profil d'utilisateur associé. |
| Faire expirer le mot de passe dans (uniquement pour les utilisateurs de comptes qui n'utilisent PAS d'IBMid pour l'authentification) | Délai pendant lequel un mot de passe doit être associé au profil utilisateur avant qu'un nouveau mot de passe ne doive être sélectionné. |
| Utilisateur parent | Compte utilisateur considéré comme utilisateur parent du profil utilisateur. Par défaut, l'utilisateur parent est l'ID de compte principal. |
| Poser des questions de sécurité | Cochez cette case si des questions de sécurité doivent être exigées lors de la connexion. Si cette option est sélectionnée, les questions de sécurité sont requises pour le profil utilisateur. |
| Mot de passe VPN | Mot de passe à utiliser pour l'accès au réseau privé virtuel. Cochez la case **Utiliser le mot de passe du portail pour le VPN** pour utiliser le mot de passe du portail client pour accéder au réseau de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} via le VPN. |
{: caption="Tableau 2. Paramètres de configuration des paramètres de connexion pour l'édition d'un profil utilisateur" caption-side="top"}

|Section|Zone|Définition|
|-------|-----|----------|
| Informations d'accès à l'API | Adresses IP autorisées | Adresses IP autorisées à s'authentifier auprès de l'API avec la clé d'API unique associée au profil utilisateur|
| Abonnements notification utilisateur | Facturation | Cochez la case **Facturation** pour recevoir une facturation par courrier électronique après sa création. |
| Questions de sécurité | Question de sécurité |Lorsque vous modifiez votre profil, vous devez répondre à cette question pour vous connecter lorsque des questions de sécurité sont activées pour votre profil. | Réponses de sécurité | Réponse | Réponse à la question de sécurité applicable (sensible à la casse). |
{: caption="Tableau 3. Autres paramètres de configuration pour l'édition d'un profil utilisateur" caption-side="top"}
Une fois que les modifications apportées à un profil utilisateur sont soumises, les changements sont immédiatement appliqués. Vous pouvez modifier à nouveau le profil utilisateur quand vous le souhaitez en répétant les étapes précédentes.

Voir [Passage à l'IBMid](/docs/account/softlayerlink.html#switching-to-ibmid) pour plus d'informations sur la configuration d'un compte IBMid.

## Edition des droits du portail client pour un utilisateur
{: #cp_editusercpperm}

Les droits d'utilisateur dans le portail client sont définis par l'administrateur du compte lors de l'ajout de l'utilisateur et peuvent être modifiés à tout moment par un utilisateur autorisé. Vous pouvez éditer votre propre profil utilisateur et, si vous êtes administrateur, certaines zones des profils utilisateur d'utilisateurs que vous avez ajoutés. Les droits sont classés selon cinq onglets : support, unités, réseau, services et compte. Vous pouvez à tout moment mettre à jour les droits d'un utilisateur mais vous devez sauvegarder vos modifications pour qu'elles deviennent actives.

Utilisez la procédure suivante pour éditer les droits d'accès au portail client d'un utilisateur.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur le nom de l'utilisateur pour accéder à son profil.
4. Cliquez sur l'icône **Autorisations** pour accéder à la fenêtre du même nom.

  Il se peut qu'un message s'affiche pour vous aviser qu'aucune modification n'a été apportée au profil utilisateur. Dans ce cas, cliquez pour ignorer les modifications et accéder à la fenêtre Droits. {: tip}

5. Sélectionnez les droits :
  * Pour définir des droits rapides, sélectionnez l'ensemble de droits dans la liste **Droits rapides**. Après avoir sélectionné un ensemble de droits, chaque droit associé à cet ensemble est affiché en orange avec une flèche orange pointant sur la case à cocher. Cliquez ensuite sur **Définir les droits** pour chaque onglet.
  * Pour définir des droits individuels, cochez ou décochez chaque case sur les onglets pour mettre à jour les droits de l'utilisateur. Cliquez sur **Sélectionner tous les droits** ou sur **Désélectionner tous les droits** sur un onglet quelconque pour sélectionner ou annuler en une fois tous les droits.
6. Cliquez sur **Modifier droits pour le portail** pour soumettre des modifications et mettre à jour les droits de l'utilisateur.
7. Pour restaurer les paramètres initiaux des droits de l'utilisateur, cliquez sur **Réinitialiser droits**. Cliquez sur **Annuler** pour annuler les changements et revenir à la fenêtre Utilisateurs.

Les droits utilisateur sont mis à jour immédiatement après que vous avez soumis les changements. Si des droits ont été octroyés, l'utilisateur peut afficher les fonctions sélectionnées ou interagir avec celles-ci. Si des droits ont été retirés, l'utilisateur ne peut pas afficher les fonctions sélectionnées ni interagir avec celles-ci. Les droits peuvent être mis à jour à tout moment en répétant les étapes précédentes. 

## Ajout d'authentification externe pour un utilisateur
{: #cp_addextauthuser}

Depuis le portail client, vous pouvez activer l'authentification externe à deux facteurs (2FA)  pour ajouter une protection lors de la connexion au portail. Cette couche supplémentaire de sécurité protège le compte contre des accès non vérifiés en garantissant que les appareils, les données et les informations de compte soient protégés. Voir [Configuration de l'authentification à deux facteurs](/docs/customer-portal/cpenable2fa.html#customerportal_2fa) pour plus d'informations.


## Changement du statut d'un utilisateur
{: #cp_changeuserstat}

Votre statut dans le portail client détermine votre accessibilité au portail client. Les catégories de statut que vous pouvez mettre à jour sur le compte incluent actif, désactivé et VPN uniquement. Votre statut peut être changé pour différentes raisons et être mis à jour à tout moment. Les catégories de statut client incluent celles que les utilisateurs peuvent mettre à jour et celles qui sont automatiquement mises à jour. Elles incluent :
<dl>
<dt>Actif</dt>
<dd>L'utilisateur dispose d'un accès complet au portail client et au VPN en fonction des droits définis par l'administrateur de compte. Ce statut peut être sélectionné manuellement ou changé à tout moment.</dd>
<dt>Désactivé</dt>
<dd>L'utilisateur n'a accès à aucun droit ou abonnement du compte, y compris au portail client et au réseau privé virtuel. Si la catégorie de statut est définie sur désactivé par un autre utilisateur du compte, ce statut peut être sélectionné manuellement ou changé à tout moment.</dd>
<dt>VPN uniquement</dt>
<dd>L'utilisateur dispose d'un accès complet à la connectivité du réseau privé virtuel (compte tenu de son ensemble de droits), mais ne peut pas accéder au portail client. Ce statut peut être sélectionné manuellement ou changé à tout moment.</dd>
<dt>Inactive</dt>
<dd>L'utilisateur n'a pas accédé au portail client ou au réseau privé virtuel au cours des 60 derniers jours. Il s'agit d'un statut généré par le système. </dd>
<dt>cancel_pending (annulation en attente)</dt>
<dd>Un administrateur du compte a annulé cet utilisateur et l'annulation est en cours de traitement. Il s'agit d'un statut généré par le système. </dd>
</dl>

Utilisez la procédure suivante pour changer le statut d'un utilisateur dans le portail client.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Utilisateurs** dans la barre de navigation.
3. Sélectionnez **Modifier statut utilisateur** dans la liste **Actions**.
4. Dans la liste **Statut**, sélectionnez le statut approprié en fonction des définitions de la liste précédente.
5. Cliquez sur **Enregistrer**.

Après que vous avez mis à jour le statut d'un utilisateur, les modifications apportées à l'accessibilité du portail client s'alignent sur le nouveau statut.


## Edition de l'accès VPN d'un utilisateur
{: #cp_edituservpnaccess}

Lorsqu'un [nouvel utilisateur est ajouté](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct), l'accès au réseau privé virtuel est sélectionné d'après diverses méthodes de connexion, notamment SSL, PPTP, ou une combinaison des deux. Avec l'accès VPN, le réseau privé est accessible dans sa totalité ou bien peut être limité à un ou plusieurs sous-réseaux spécifiques. Vous pouvez gérer et mettre à jour l'accès VPN à tout moment depuis la fenêtre Utilisateurs. Utilisez la procédure suivante pour éditer l'accès VPN d'un utilisateur.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Accès VPN** dans la barre de navigation.
3. Dans la colonne **Accès VPN** de l'utilisateur, cliquez sur le lien du type d'accès en cours pour afficher la fenêtre Accès VPN.
4. Dans la liste **Type de VPN**, sélectionnez une méthode VPN (SSL, PPTP, SSL et PPTP, ou aucune) à affecter à l'utilisateur.
5. Indiquez comment gérer l'**Accès au sous-réseau** :
  * Sélectionnez **Auto** pour gérer automatiquement l'accès au sous-réseau.
  * Sélectionnez **Manuel** pour gérer manuellement l'accès au sous-réseau, puis cochez la case **Autoriser accès** pour chaque sous-réseau auquel l'utilisateur doit avoir accès. Prenez soin de décocher les cases correspondant aux sous-réseaux auxquels l'utilisateur ne doit pas avoir accès.
6. Cliquez sur **Enregistrer**.

Après que l'accès VPN d'un utilisateur a été mis à jour, ses droits sont mis à jour et la colonne Accès VPN affiche la méthode d'accès VPN mise à jour, le cas échéant.

### Activation ou désactivation de l'accès VPN
{: #cp_pptpvpn}

Vous pouvez activer le VPN PPTP afin de former un tunnel sécurisé d'accès au réseau privé de l'infrastructure {{site.data.keyword.BluSoftlayer_full}} à l'aide d'un logiciel client spécialisé s'exécutant sur votre bureau ou une unité dédiée. Vous pouvez utiliser PPTP si vous avez besoin de connecter votre bureau complet ou si vous ne pouvez pas utiliser la solution de réseau privé virtuel sous SSL.

Une connexion PPTP vous est allouée avec des connexions supplémentaires disponibles. Vous pouvez demander une aide pour activer l'accès PPTP illimité, disponible sans frais supplémentaires. Utilisez la procédure suivante pour activer l'accès VPN PPTP.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Accès VPN** dans la barre de menus.
3. Dans la colonne **Accès VPN** de l'utilisateur, cliquez sur le lien du type d'accès en cours pour afficher la fenêtre Accès VPN.
4. Dans la liste **Type de VPN**, sélectionnez une méthode VPN (SSL, PPTP, SSL et PPTP, ou aucune) à affecter à l'utilisateur.


## Sélection de notifications par courrier électronique
{: #cp_select-email-notifications}

Vous pouvez sélectionner les notifications par courrier électronique que vous souhaitez recevoir de la part de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} et celles que vous ne souhaitez pas recevoir. Par défaut, vous recevez toutes les notifications par courrier électronique, mais vous pouvez les modifier à tout moment. Pour modifier vos paramètres de notification par courrier électronique, procédez comme suit :
1. Accédez au portail client à l'aide de vos données d'identification uniques pour le compte associé à l'adresse électronique destinataire des notifications.
2. Cliquez sur **Compte** > **Utilisateurs** > **Préférences de courrier électronique** dans la barre de menus.
3. Dans la liste de types de notification, désélectionnez les notifications que vous ne souhaitez plus recevoir.

Vos modifications sont sauvegardées automatiquement. Ces paramètres affectent le courrier électronique qui vous est envoyé, mais ils n'ont aucun impact sur les notifications par courrier électronique des autres utilisateurs de votre compte.


## Définition de l'option Support dans l'Union européenne
{: #cp_seteusupported}

Vous pouvez indiquer que vous souhaitez l'aide exclusive d'une équipe de support physiquement située dans l'Union européenne (UE). Vous pouvez sélectionner cette option lorsque vous configurez votre compte ou quand vous le mettez à jour. Pour définir l'option **Support dans l'Union européenne**, utilisez la procédure suivante :
1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez sur **Compte** > **Gérer** > **Profil de la Société** dans la barre de menus.
3. Cochez la case **Support dans l'Union européenne**.
4. Cliquez sur **Demander mise à jour du profil**.

Si l'option **Support dans l'Union européenne** n'est pas disponible, il est possible que l'accès VPN PPTP de certains utilisateurs de votre compte soit activé. Désactivez d'abord l'accès de réseau privé virtuel sous PPTP pour tous les utilisateurs pour pouvoir activer l'option **Support dans l'Union européenne**. Pour plus d'informations, voir [Activation ou désactivation de l'accès VPN PPTP](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn).

Pour plus d'informations sur la mise en oeuvre de l'option **Support dans l'Union européenne** lorsque vous ouvrez un ticket de demande de service, voir [Demande de support pour des ressources dans l'Union européenne](/docs/get-support/howtogetsupport.html#eusupported).
