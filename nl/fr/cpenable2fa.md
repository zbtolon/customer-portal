---

copyright:

  years: 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Configuration de l'authentification à deux facteurs
{: #customerportal_2fa}

Dans le portail client, une authentification à deux facteurs externe (2FA) peut être activée pour ajouter une protection supplémentaire lorsque vous vous connectez au portail. Cette couche supplémentaire de sécurité protège le compte contre des accès non vérifiés en garantissant que les appareils, les données et les informations de compte soient protégés.
{:shortdesc}

Si vous activez l'authentification à deux facteurs (2FA) dans le portail client pour votre compte SoftLayer existant, vous devez entrer votre code de sécurité lorsque vous vous connectez à la console {{site.data.keyword.Bluemix_notm}}. L'authentification à deux facteurs ne s'applique qu'aux ressources d'infrastructure de votre compte {{site.data.keyword.Bluemix_notm}}. Vous pouvez effectuer différentes actions sur les ressources de votre compte {{site.data.keyword.Bluemix_notm}} sans vous soumettre à l'authentification à deux facteurs.

L'authentification à deux facteurs pour votre compte SoftLayer ne s'effectue pas par IBMid, mais toujours par compte. Lorsqu'un IBMid est associé à plusieurs comptes et que vous passez d'un compte à l'autre, vous devez confirmer votre identité chaque fois que vous utilisez un compte différent. Vous devez confirmer votre identité lorsque vous basculez entre des comptes même si le précédent et le nouveau ont tous deux été configurés avec le même mécanisme 2FA.

## Activation de l'authentification à deux facteurs

L'authentification à deux facteurs est disponible sous deux formes. Les deux méthodes d'authentification externe peuvent être ajoutées pour chaque utilisateur, pour un faible coût mensuel :

* Symantec Identity Protection est l'outil d'authentification externe le plus couramment utilisé et offre un code de sécurité dynamique utilisé en plus du nom d'utilisateur et du mot de passe lors de l'accès au portail client.
* L'authentification PhoneFactor offre une authentification externe avec un appel téléphonique, un SMS ou une application mobile.

 Si vous disposez d'un compte lié, vous pouvez bénéficier de l'authentification multi-facteur en [activant l'authentification multi-facteur](/docs/iam/mfa.html) pour l'ensemble de votre compte {{site.data.keyword.Bluemix_notm}}.
 {: tip}

Pour configurer l'authentification à deux facteurs, procédez comme suit :

1. Accédez à l'écran **Utilisateurs** dans le portail client.
2. Sélectionnez **Ajouter authentification externe** depuis le menu **Actions** pour l'utilisateur concerné.
3. En fonction du type d'authentification externe commandé, procédez comme suit :
    * Si vous choisissez Symantec Identity Protection, sélectionnez **Symantec Identity Protection** et entrez les données d'identification de l'utilisateur.
    * Si vous choisissez PhoneFactor, sélectionnez **PhoneFactor**.
4. Cliquez sur **Continuer**
5. Suivez les invites à l'écran pour **Code promo** et **Accusé de réception MSA**.
6. Cliquez sur **Commander Module d'Authentification Externe** pour terminer la commande. Cliquez sur **Annuler** pour annuler l'action.

## Etapes suivantes
{: #2fanextsteps}

Après que vous avez ajouté l'authentification externe pour un utilisateur, les prochaines étapes dépendent du type d'authentification.
* Si Symantec Identity Protection est activé, vous devez ajouter le code de sécurité associé à l'ID des Données d'Identification de l'utilisateur. Il s'agit du code de sécurité saisi dans le système lorsque Symantec Identity Protection a été ajouté au compte.
* Si PhoneFactor est activé, l'utilisateur doit activer PhoneFactor pour utiliser ce type d'authentification à deux facteurs avec le compte.

### Activation de l'authentification PhoneFactor
{: #cp_actphonefacauth}

Après que vous avez ajouté PhoneFactor, vous devez activer manuellement l'authentification externe avec PhoneFactor via le portail client. Dans la mesure où PhoneFactor utilise le contact manuel, il est important de s'assurer que tous les numéros de téléphone associés au compte restent toujours à jour. Si les informations de contact ne sont pas à jour, vous risquez de ne pas pouvoir accéder au portail client et au VPN quand PhoneFactor est actif. Une fois que PhoneFactor a été ajouté, vous recevrez un e-mail confirmant son ajout. Une fois l'e-mail reçu, utilisez la procédure suivante pour activer l'authentification PhoneFactor.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte > Utilisateurs** dans la barre de navigation.
3. Cliquez sur le nom d'utilisateur pour accéder au profil utilisateur associé pour cet utilisateur.
4. Faites défiler jusqu'à la section **Paramètres PhoneFactor**.

  Si la section Paramètres PhoneFactor n'est pas disponible, commencez par vérifier que vous avez bien reçu l'e-mail confirmant la mise à disposition de PhoneFactor. Si PhoneFactor a été mis à disposition mais que la section n'est pas disponible, créez un ticket de demande de service. Si PhoneFactor n'a pas encore été mis à disposition, attendez de recevoir l'e-mail, puis réessayez.
  {: tip}

5. Sélectionnez **Actif** dans la liste **Statut**.
6. Editez le **numéro de téléphone principal** pour l'authentification.
  1. Cliquez sur le lien **Editer**.
  2. Entrez les **Code pays**, **Numéro de téléphone** et **Extension**, le cas échéant, dans les zones associées.
  3. Cliquez sur **Authentifier et sauvegarder le numéro** pour terminer l'authentification;

    Lors de l'ajout d'un numéro de téléphone pour l'authentification, vous devez rester à côté du téléphone. Une fois que vous avez cliqué sur **Authentifier**, le numéro est appelé et vous êtes invité à exécuter une étape pour authentifier le numéro. Les numéros de téléphone ne peuvent pas être authentifiés sans l'exécution de ces étapes.
    {: tip}

  4. Pour ajouter un **Numéro de téléphone secondaire**, répétez la procédure.
7. Sélectionnez la **méthode de contact** dans la liste **Méthode**.
8. Sélectionnez un **Type de code confidentiel** dans la liste **Type de code confidentiel**.
9. Si vous sélectionnez **Unique** > **Valeur de code confidentiel**, entrez le code confidentiel dans la zone **Valeur de code confidentiel**.
10. Cliquez sur **Mettre à jour** pour mettre à jour les changements et activer l'authentification PhoneFactor.

Une fois que PhoneFactor est activé, l'authentification via PhoneFactor est obligatoire pour le portail client ou le VPN. Après l'authentification avec les données d'identification de l'utilisateur, un message vous indique qu'une tentative d'authentification par PhoneFactor est en cours. Vous, ou l'utilisateur que vous ajoutez, devez être à proximité du téléphone indiqué pour PhoneFactor afin de compléter l'authentification. PhoneFactor tente de vous authentifier cinq fois. Au bout de cinq tentatives infructueuses, vous êtes verrouillé pendant environ une heure. Vous, ou un utilisateur dotés d'un accès administrateur au compte, pouvez à tout moment changer les paramètres d'authentification PhoneFactor. Vous, ou un administrateur du compte, pouvez à tout moment désactiver PhoneFactor.

 Si vous choisissez de configurer PhoneFactor pour le portail client et votre connexion VPN, il en découle deux processus de connexion 2FA distincts, l'un pour le portail client et l'autre pour le VPN.
 {: tip}

#### Méthodes d'authentification PhoneFactor
{: #cp_phonefacauthmeths}

Si vous configurez PhoneFactor comme type d'authentification, vous pouvez choisir l'une des options suivantes comme méthode d'authentification :

<dl>
<dt>Appel téléphonique et standard (pas de code confidentiel)</dt>
<dd>Avec cette option, lorsque vous vous connectez au portail, vous recevez un appel téléphonique sur le numéro principal activé. Lorsque vous répondez à l'appel, il vous est demandé d'appuyer sur la touche dièse (#) pour terminer l'authentification.</dd>
<dt>Appel téléphonique avec code confidentiel</dt>
<dd>Avec cette option, vous entrez une valeur de code confidentiel sur le portail client. Le code confidentiel doit comporter entre 4 et 8 chiffres. Lorsque vous essayez de vous connecter au portail, vous recevez un appel sur le numéro de téléphone principal figurant sur le portail. Lorsque vous répondez, vous êtes invité à entrer votre numéro d'identification personnel suivi du signe # pour terminer l'authentification. </dd>
<dt>SMS et code confidentiel unique</dt>
<dd>Avec cette option, vous recevez un message texte avec un code confidentiel à utiliser pour répondre au message. Lorsque vous entrez le code confidentiel fourni, le processus d'authentification aboutit et vous connecte au portail.</dd>
<dt>SMS avec valeur de code confidentiel unique</dt>
<dd>Avec cette option, vous créez une valeur de code confidentiel comportant de 4 à 8 chiffres. Après avoir reçu ce message texte, répondez avec le code fourni et votre numéro de code confidentiel sans espaces.</dd>
<dt>Application PhoneFactor et standard (pas de code confidentiel)</dt>
<dd>Ouvrez l'application PhoneFactor (Microsoft Authenticator) sur votre appareil et cliquez sur <strong>Authentifier</strong>. Un message s'affiche pour indiquer que vous vous êtes authentifié à l'aide de PhoneFactor et vous êtes connecté au portail.</dd>
<dt>Application PhoneFactor avec code confidentiel</dt>
<dd>Avec cette option, vous définissez un code confidentiel, composé de 4 à 8 chiffres, sur le portail. Vous ouvrez ensuite l'application PhoneFactor (Microsoft Authenticator) sur votre appareil. Vous entrez ensuite votre code confidentiel créé sur le portail et cliquez sur <strong>Authentifier</strong> pour vous connecter au portail.</dd>
</dl>
