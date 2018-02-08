---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-17"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestion d'un profil utilisateur
{: #customerportal_accuserprof}

Sur le portail client, un profil utilisateur comporte différentes données sur l'utilisateur, y compris les informations de contact et la clé d'API. C'est également là que sont stockés les mots de passe. En outre, si vous disposez d'un accès administrateur, vous pouvez changer les droits et l'accès à l'unité depuis le profil.
{:shortdesc}

Dans le profil utilisateur, vous pouvez gérer les informations de contact et les mots de passe, afficher les clés d'API et mettre à jour des droits supplémentaires et l'accès à l'unité en fonction de vos droits.

## Edition d'un profil utilisateur
{: #cp_edituserprofile}

Après qu'un profil utilisateur a été créé sur le portail client, vous pouvez l'éditer à tout moment. Les détails associés au profil utilisateur incluent les informations personnelles, les paramètres de connexion, les détails d'accès aux API, les abonnements aux notifications utilisateur ainsi que les questions de sécurité. Utilisez la procédure suivante pour éditer un profil utilisateur.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur le nom d'utilisateur pour accéder au profil utilisateur associé pour cet utilisateur.
4. Editez les détails du **Profil utilisateur** selon les besoins. Pour les utilisateurs de comptes utilisant IBMid pour l'authentification, mettez à jour vos adresse e-mail et mot de passe dans votre profil IBMid. voir le Tableau 1 pour plus d'informations.
5. Si vous souhaitez réinitialiser votre mot de passe après vous être connecté, cliquez sur **Réinitialiser mot de passe** pour générer un e-mail vous permettant de changer votre mot de passe. 
6. Cliquez sur **Editer l'utilisateur** pour soumettre les modifications.

| Zone | Définition |
|-----|----------|
| Prénom, Nom | Prénom et nom de l'utilisateur associé au profil utilisateur.|
| Adresse e-mail | Adresse e-mail préférée pour la réception des notifications de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} concernant le compte. La modification de l'adresse e-mail change l'enregistrement dans l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Ce changement n'affecte pas le lien vers les données d'authentification IBMid. Vous devez modifier l'adresse e-mail pour l'IBMid depuis le profil IBMid.|
| Fuseau horaire| Fuseau horaire à utiliser de préférence lors de l'affichage des données horodatées.|
| Téléphone, Autre téléphone| Numéros de téléphone préférés à utiliser par l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.|
| Rue, Ville, Pays, Etat/Province, Code postal | Adresse complète du contact, à utiliser par l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.|
{: caption="Tableau 1. Paramètres de configuration des informations personnelles pour l'édition d'un profil utilisateur" caption-side="top"}

|Zone|Définition|
|-----|----------|
| Limiter l'accès à l'adresse IP | Adresse IP à laquelle limiter l'accès lors de tentatives d'utilisation du portail client sous le profil utilisateur associé. |
| Faire expirer le mot de passe dans (uniquement pour les utilisateurs de comptes qui n'utilisent PAS d'IBMid pour l'authentification) | Durée pendant laquelle un mot de passe doit être associé au profil utilisateur avant qu'un nouveau mot de passe ne doive être sélectionné. |
| Utilisateur parent | Compte utilisateur considéré comme utilisateur parent du profil utilisateur. Par défaut, l'utilisateur parent est l'ID de compte principal. |
| Poser des questions de sécurité | Cochez cette case quand des questions de sécurité sont obligatoires lors de la connexion. Si cette option est sélectionnée, les questions de sécurité sont requises pour le profil utilisateur. |
| Mot de passe VPN | Mot de passe à utiliser pour l'accès au réseau privé virtuel. Cochez la case **Utiliser le mot de passe du portail pour le VPN** pour utiliser le mot de passe du portail client pour accéder au réseau de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} via le VPN. |
{: caption="Tableau 2. Paramètres de configuration des paramètres de connexion pour l'édition d'un profil utilisateur" caption-side="top"}

|Section|Zone|Définition|
|-------|-----|----------|
| Informations d'accès à l'API | Adresses IP autorisées | Adresses IP autorisées pour l'authentification auprès de l'API via la clé d'API unique associée au profil utilisateur. |
| Abonnements notification utilisateur | Facturation | Cochez la case **Facturation** pour recevoir une facture par e-mail une fois celle-ci créée. |
| Questions de sécurité | Question de sécurité | Lors de l'édition de votre profil, il s'agit de la question à laquelle vous devez répondre pour vous connecter quand les questions de sécurité ont été activées pour votre profil.
| Réponses de sécurité | Réponse | Réponse à la question de sécurité applicable ; sensible à la casse. |
{: caption="Tableau 3. Autres paramètres de configuration pour l'édition d'un profil utilisateur" caption-side="top"}
Une fois que les modifications apportées à un profil utilisateur sont soumises, les changements sont immédiatement appliqués. Vous pouvez modifier à nouveau le profil utilisateur quand vous le souhaitez en répétant les étapes précédentes.   

Voir [Passage à l'IBMid](/docs/account/softlayerlink.html#switching-to-ibmid) pour plus d'informations sur la configuration d'un compte IBMid.

## Edition des droits du portail client pour un utilisateur
{: #cp_editusercpperm}

Les droits utilisateur sur le portail client sont définis par l'administrateur de compte lorsque l'utilisateur est ajouté ; ils peuvent être édités à tout moment par un utilisateur autorisé. Vous pouvez éditer votre propre profil utilisateur et, si vous êtes administrateur, certaines zones des profils utilisateur d'utilisateurs que vous avez ajoutés. Les droits sont classés selon cinq onglets : support, unités, réseau, services et compte. Vous pouvez à tout moment mettre à jour les droits d'un utilisateur mais vous devez sauvegarder vos modifications pour qu'elles deviennent actives. 

Utilisez la procédure suivante pour éditer les droits d'accès au portail client d'un utilisateur. 

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur le nom de l'utilisateur pour accéder à son profil.
4. Cliquez sur l'icône **Autorisations** pour accéder à la fenêtre du même nom. 

  Il est possible que vous receviez un message indiquant que des changements n'ont pas été sauvegardés dans le profil utilisateur. Si aucune modification n'a été apportée au profil, cliquez pour annuler les changements et accéder à la fenêtre Autorisations.
  {: tip}

5. Sélectionnez les droits :
  * Pour définir des droits rapides, sélectionnez l'ensemble de droits dans la liste **Droits rapides**. Une fois que vous avez sélectionné un ensemble, chaque droit associé à l'ensemble s'affiche en orange, avec une flèche orange pointant sur la case à cocher. Cliquez ensuite sur **Définir droits** pour chaque onglet. 
  * Pour définir des droits individuels, cochez ou décochez chaque case dans les onglets pour mettre à jour les droits de l'utilisateur. Sur un onglet, cliquez pour **sélectionner tous les droits** ou **désélectionner tous les droits** en une fois. 
6. Cliquez sur **Modifier droits pour le portail** pour soumettre des modifications et mettre à jour les droits de l'utilisateur.
7. Pour restaurer les paramètres initiaux des droits de l'utilisateur, cliquez sur **Réinitialiser droits**. Cliquez sur **Annuler** pour annuler les changements et revenir à la fenêtre Utilisateurs. 

Les droits utilisateur sont mis à jour immédiatement après que vous avez soumis les changements. Si des droits ont été octroyés, l'utilisateur peut afficher les fonctions sélectionnées ou interagir avec ces dernières. Si des droits ont été retirés, l'utilisateur ne peut plus afficher les fonctions sélectionnées ou interagir avec ces dernières. Les droits peuvent à tout moment être à nouveau mis à jour en répétant la procédure précédente.

## Ajout d'authentification externe pour un utilisateur
{: #cp_addextauthuser}

Depuis le portail client, vous pouvez activer l'authentification externe à deux facteurs pour ajouter une protection supplémentaire lors de la connexion au portail. Cette couche supplémentaire de sécurité protège le compte des accès non vérifié en garantissant que les appareils, données et les informations de compte sont protégés. Cette authentification externe est disponible sous les formes suivantes :

* **Symantec Identity Protection** est l'outil d'authentification externe le plus couramment utilisé et offre un code de sécurité dynamique utilisé en plus des nom d'utilisateur et mot de passe lors de l'accès au portail client.
* L'authentification **PhoneFactor** offre une authentification d'utilisateur externe depuis un téléphone, un SMS ou une application mobile. PhoneFactor requiert un numéro de téléphone valide auquel vous devez avoir accès à chaque fois que vous tentez de vos authentifier. 

Vous pouvez ajouter les deux méthodes d'authentification externe, par utilisateur, pour un [faible coût mensuel ![Icône de lien externe](../icons/launch-glyph.svg)](http://www.softlayer.com/services/security/){:new_window}. Utilisez la procédure suivante pour ajouter une authentification externe pour un utilisateur du portail client.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Sélectionnez **Ajouter authentification externe** depuis la liste **Actions** de l'utilisateur.
4. Sélectionnez le type d'authentification externe à commander.
  * **Symantec Identity Protection** -- Entrez l'ID des données d'identification de l'utilisateur dans la zone **Données d'Identification**.
  * **PhoneFactor** -- Choisissez une [méthode d'authentification](#cp_phonefacauthmeths).
5. Cliquez sur **Continuer**
6. Suivez les invites à l'écran pour le **Code Promo** et **MSA Acknowledgement**.
7. Cliquez sur **Commander Module d'Authentification Externe** pour terminer la commande. 

Après que vous avez ajouté l'authentification externe pour un utilisateur, les prochaines étapes dépendent du type d'authentification.
* Si Symantec Identity Protection est activé, vous devez ajouter le code de sécurité associé à l'ID de données d'identification de l'utilisateur de l'utilisateur qui a été entré dans le système au moment où Symantec Identity Protection a été ajouté au compte.
* Si PhoneFactor est activé, l'utilisateur doit [activer PhoneFactor](#cp_actphonefacauth) pour utiliser ce type d'authentification à deux facteurs avec le compte.

### Activation de l'authentification PhoneFactor 
{: #cp_actphonefacauth}

Après que vous avez ajouté PhoneFactor, vous devez activer manuellement l'authentification externe avec PhoneFactor via le portail client. Parce que PhoneFactor utilise le contact manuel, il est important de s'assurer que tous les numéros de téléphone associés au compte restent toujours à jour. Si les informations de contact ne sont pas mise à jour, vous risquez de ne pas pouvoir accéder au portail client et au VPN quand PhoneFactor est actif. Une fois que PhoneFactor a été ajouté, vous recevez un e-mail de confirmation de l'ajout de PhoneFactor. Une fois l'e-mail reçu, utilisez la procédure suivante pour activer l'authentification PhoneFactor.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur le nom d'utilisateur pour accéder au profil utilisateur associé pour cet utilisateur.
4. Faites défiler jusqu'à la section **Paramètres PhoneFactor**.

  Si la section Paramètres PhoneFactor n'est pas disponible, commencez par vérifier que vous avez bien reçu l'e-mail indiquant la mise à disposition de PhoneFactor. Si PhoneFactor a été mis à disposition mais que la section n'est pas disponible, créez un ticket de demande de service. Si PhoneFactor n'a pas encore été mis à disposition, attendez de recevoir l'e-mail puis réessayez. Si PhoneFactor n'a pas encore été ajouté, voir [Ajout d'une authentification externe pour un utilisateur](/docs/customer-portal/cpmanuserprof.html#cp_addextauthuser).
  {: tip}

5. Sélectionnez **Actif** dans la liste **Statut**. 
6. Editez le **numéro de téléphone principal** pour l'authentification.
  1. Cliquez sur le lien **Editer**. 
  2. Entrez les **Code pays**, **Numéro de téléphone** et **Extension**, le cas échéant, dans les zones associées.
  3. Cliquez sur **Authentifier et sauvegarder le numéro** pour terminer l'authentification;

    Lors de l'ajout d'un numéro de téléphone pour l'authentification, vous devez être à côté du téléphone. Une fois que vous avez cliqué sur **Authentifier**, le numéro est appelé et vous êtes invité à exécuter une étape pour authentifier le numéro. Les numéros de téléphone ne peuvent pas être authentifiés sans l'exécution de ces étapes.{: tip}

  4. Pour ajouter un **Numéro de téléphone secondaire**, répétez la procédure. 
7. Sélectionnez la **méthode de contact** dans la liste **Méthode**.
8. Sélectionnez un **Type de code confidentiel** dans la liste **Type de code confidentiel**.
9. Si vous sélectionnez **Unique** > **Valeur de code confidentiel**, entrez le code confidentiel dans la zone **Valeur de code confidentiel**.
10. Cliquez sur **Mettre à jour** pour mettre à jour les changements et activer l'authentification PhoneFactor.

Une fois que PhoneFactor est activé, l'authentification via PhoneFactor est obligatoire pour le portail client ou le VPN. Après l'authentification avec les données d'identification de l'utilisateur, un message vous indique que l'authentification PhoneFactor est en cours. Vous, ou l'utilisateur que vous ajoutez, devez être à proximité du téléphone indiqué pour PhoneFactor afin de compléter l'authentification. PhoneFactor tente de vous authentifier cinq fois. Au bout de cinq tentatives infructueuses, vous êtes verrouillé pendant environ une heure. Vous, ou un utilisateur dotés d'un accès administrateur au compte, pouvez à tout moment changer les paramètres d'authentification PhoneFactor. Vous, ou un administrateur du compte, pouvez à tout moment désactiver PhoneFactor. 

#### Méthodes d'authentification PhoneFactor
{: #cp_phonefacauthmeths}

Si vous configurez PhoneFactor comme type d'authentification, vous pouvez choisir l'une des options suivantes comme méthode d'authentification :
<dl>
<dt>Appel téléphonique et standard (pas de code confidentiel)</dt>
<dd>Avec cette option, lorsque vous vous connectez au portail, vous recevez un appel téléphonique sur le numéro principal activé. Lorsque vous répondez à l'appel, il vous est demandé d'appuyer sur la touche dièse (#) pour terminer l'authentification.</dd>
<dt>Appel téléphonique avec code confidentiel</dt>
<dd>Avec cette option, vous entrez une valeur de code confidentiel sur le portail client. La code confidentiel doit comporter entre 4 et 8 chiffres. Lorsque vous essayez de vous connecter au portail, vous recevez un appel sur le numéro de téléphone principal figurant sur le portail. Quand vous répondez, il vous est demandé d'appuyer sur la touche dièse (#) pour terminer l'authentification.</dd>
<dt>SMS et code confidentiel unique</dt>
<dd>Avec cette option, vous recevez un message texte avec un code confidentiel à utiliser pour répondre au message. Quand vous entrez le code confidentiel fourni, le processus d'authentification aboutit et vous connecte au portail.</dd>
<dt>SMS avec valeur de code confidentiel unique</dt>
<dd>Avec cette option, vous créez une valeur de code confidentiel comportant de 4 à 8 chiffres. Lorsque vous recevez un message texte, vous répondez avec le code fourni et votre numéro de code confidentiel sans espaces. </dd>
<dt>Application PhoneFactor et standard (pas de code confidentiel)</dt>
<dd>Ouvrez l'application PhoneFactor (Azure Authenticator) sur votre appareil et cliquez sur <strong>Authentifier</strong>. Un message s'affiche pour indiquer que vous vous êtes authentifié à l'aide de PhoneFactor et vous êtes connecté au portail.</dd>
<dt>Application PhoneFactor avec code confidentiel</dt>
<dd>Avec cette option, vous définissez un code confidentiel, entre 4 et 8 chiffres, sur le portail. Vous ouvrez ensuite l'application PhoneFactor (Azure Authenticator) sur votre appareil. Vous entrez ensuite votre code confidentiel créé sur le portail et cliquez sur <strong>Authentifier</strong> pour vous connecter au portail.</dd>
</dl>

## Changement du statut d'un utilisateur
{: #cp_changeuserstat}

Votre statut sur le portail client détermine votre accessibilité au portail. Les catégories de statut que vous pouvez mettre à jour sur le compte incluent actif, désactivé et VPN uniquement. Votre statut peut être changé pour différentes raisons, et il peut être mis à jour à tout moment. Les catégories de statut client incluent celles que les utilisateurs peuvent mettre à jour et celles qui sont automatiquement mises à jour. Elles incluent :
<dl>
<dt>Actif</dt>
<dd>L'utilisateur dispose d'un accès complet au portail client et au VPN en fonction des droits définis par l'administrateur de compte. Ce statut peut être sélectionné manuellement ou changé à tout moment.</dd>
<dt>Désactivé</dt>
<dd>L'utilisateur n'a pas accès aux droits ou abonnements du compte, y compris le portail client et le VPN. Si la catégorie de statut est définie sur désactivé par un autre utilisateur du compte, ce statut peut être sélectionné manuellement ou changé à tout moment.</dd>
<dt>VPN uniquement</dt>
<dd>L'utilisateur dispose d'un accès complet à la connectivité VPN, en fonction de son ensemble de droits, mais il ne peut pas accéder au portail client. Ce statut peut être sélectionné manuellement ou changé à tout moment.</dd>
<dt>Inactive</dt>
<dd>L'utilisateur n'a pas accédé au portail client ou au VPN au cours des 60 derniers jours. Il s'agit d'un statut généré par le système.</dd>
<dt>cancel_pending (annulation en attente)</dt>
<dd>Un administrateur du compte a annulé cet utilisateur et l'annulation est en cours de traitement. Il s'agit d'un statut généré par le système.</dd>
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

Quand un [nouvel utilisateur est ajouté](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct) à un compte de portail client, l'accès VPN est sélectionné à partir de différentes méthodes de connexion, notamment SSL, PPTP, ou une combinaison des deux. Avec l'accès VPN, le réseau privé est accessible dans sa totalité ou bien peut être limité à un ou plusieurs sous-réseaux spécifiques. Vous pouvez gérer et mettre à jour l'accès VPN à tout moment depuis la fenêtre Utilisateurs. Utilisez la procédure suivante pour éditer l'accès VPN d'un utilisateur.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Accès VPN** dans la barre de navigation.
3. Dans la colonne **Accès VPN** de l'utilisateur, cliquez sur le lien du type d'accès en cours pour afficher la fenêtre Accès VPN.
4. Dans la liste **Type de VPN**, sélectionnez une méthode VPN (SSL, PPTP, SSL & PPTP, ou aucune) à affecter à l'utilisateur.
5. Indiquez comment l'**Accès au sous-réseau** doit être géré :
  * Sélectionnez **Auto** pour gérer automatiquement l'accès au sous-réseau.
  * Sélectionnez **Manuel** pour gérer manuellement l'accès au sous-réseau, puis cochez la case **Autoriser accès** pour chaque sous-réseau auquel l'utilisateur doit avoir accès. Veillez à décocher les cases correspondant aux sous-réseaux auxquels l'utilisateur ne doit pas avoir accès.
6. Cliquez sur **Enregistrer**.

Après que l'accès VPN d'un utilisateur a été mis à jour, les droits sont mis à jour en conséquence et la colonne Accès VPN affiche la méthode d'accès VPN mise à jour, le cas échéant.

### Activation ou désactivation de l'accès VPN 
{: #cp_pptpvpn}

Vous pouvez activer le VPN PPTP afin de former un tunnel sécurisé d'accès au réseau privé de l'infrastructure {{site.data.keyword.BluSoftlayer_full}} à l'aide d'un logiciel client spécialisé s'exécutant sur votre bureau ou une unité dédiée. Vous pouvez utiliser PPTP si vous avez besoin de connecter la totalité de votre bureau ou si vous ne pouvez pas utiliser la solution VPN SSL.

Une connexion PPTP vous est allouée avec des connexions supplémentaires disponibles. Vous pouvez demander une aide pour activer l'accès PPTP illimité, disponible sans frais supplémentaires. Utilisez la procédure suivante pour activer l'accès VPN PPTP.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Accès VPN** dans la barre de menus.
3. Dans la colonne **Accès VPN** de l'utilisateur, cliquez sur le lien du type d'accès en cours pour afficher la fenêtre Accès VPN.
4. Dans la liste **Type de VPN**, sélectionnez une méthode VPN (SSL, PPTP, SSL & PPTP, ou aucune) à affecter à l'utilisateur.

## Définition de l'option Support dans l'Union européenne
{: #cp_seteusupported}

Vous pouvez indiquer que vous souhaitez l'aide exclusive d'une équipe de support physiquement située dans l'Union européenne (UE). Vous pouvez sélectionner cette option lorsque vous configurez votre compte ou quand vous le mettez à jour. Pour définir l'option **Support dans l'Union européenne**, utilisez la procédure suivante :
1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez sur **Compte** > **Gérer** > **Profil de la Société** dans la barre de menus.
3. Cochez la case **Support dans l'Union européenne**.
4. Cliquez sur **Demander mise à jour du profil**.

Si l'option **Support dans l'Union européenne** n'est pas disponible, il est possible que l'accès VPN PPTP de certains utilisateurs de votre compte soit activé. Désactivez l'accès VPN PPTP pour tous les utilisateurs de votre compte avant d'activer l'option **Support dans l'Union européenne**. Voir [Activation ou désactivation de l'accès VPN PPTP](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn) pour plus d'informations.

Pour plus d'informations sur la mise en oeuvre de l'option **Support dans l'Union européenne** lorsque vous ouvrez un ticket de demande de service, voir [Demande de support pour des ressources dans l'Union européenne](/docs/get-support/howtogetsupport.html#eusupported).
