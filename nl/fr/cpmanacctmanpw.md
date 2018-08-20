---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-13"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestion des mots de passe
{: #customerportal_manpws}

Si vous êtes utilisateur principal ou propriétaire d'un compte, vous pouvez activer le suivi des mots de passe, ainsi que configurer un mot de passe à usage ponctuel pour le compte. Le suivi des mots de passe permet aux utilisateurs de stocker les données de mot de passe logiciel pour des appareils et leur logiciel associé.
{:shortdesc}

## Activation du suivi des mots de passe
{: #customerportal_enabpwtrak}

Le portail client comporte un outil facultatif de suivi du mot de passe pour chaque compte. Vous pouvez utiliser cet outil pour extraire votre nom d'utilisateur et votre mot de passe si vous avez perdu ou oublié ces informations.

Les équipes de support utilisent également le suivi des mots de passe si l'accès distant à un système est requis. Les noms d'utilisateur et les mots de passe ne sont utilisés par le support que lorsque ceci est nécessaire.

Le suivi des mots de passe dans le portail client est facultatif. Tout utilisateur disposant des droits appropriés peut examiner tous les mots de passe stockés par cet outil. Les informations d'utilisateur et de mot de passe sont suivies manuellement de façon à ne pas être automatiquement synchronisées avec un appareil ou son logiciel. Par conséquent, veillez à mettre à jour l'outil de suivi des mots de passe lorsque que vous mettez à jour les utilisateurs et les mots de passe sur les appareils et logiciels. Utilisez la procédure suivante pour ajouter un utilisateur à l'outil de suivi des mots de passe.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez dans le menu sur **Périphériques** > **Gérer** > **Mots de passe**.
3. Cliquez sur l'onglet **Ajouter identifiants**.
4. Sélectionnez dans la liste **Nom du périphérique** celui auquel l'utilisateur est associé.
5. Sélectionnez dans la liste **Logiciels** celui auquel l'utilisateur est associé.

  Le logiciel répertorié est fourni par l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} via des abonnements payants ou gratuits. Aucun logiciel tiers installé manuellement sur l'appareil n'est disponible pour suivi via le portail client.
  {: tip}

6. Entrez le nom d'utilisateur et le mot de passe pour le logiciel dans les zones appropriées.
8. Facultatif : Vous pouvez entrer tout commentaire adéquate dans la zone **Remarques**.
9. Cliquez sur **Ajouter identifiants**.

Une fois l'utilisateur ajouté, les informations sont stockées dans l'outil jusqu'à leur suppression manuelle. Par défaut, toutes les combinaisons de nom d'utilisateur et de mot de passe sont stockées en fonction du nom de l'appareil. Les entrées sont affichées par ordre alphabétique, par nom d'appareil puis par nom d'utilisateur.

### Filtrage des informations dans l'outil de suivi des mots de passe
{: #cp_filterusinfopwtracktool}

Pour afficher, éditer ou supprimer des informations utilisateur, vous pouvez appliquer un filtre afin de localiser rapidement un utilisateur. Ce filtrage est pratique lorsque la liste des utilisateurs couvre de nombreuses lignes ou pages. Utilisez la procédure suivante pour filtrer par appareil, logiciel ou utilisateur dans l'outil de suivi des mots de passe.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez dans le menu sur **Périphériques** > **Gérer** > **Mots de passe**.
3. Cliquez sur l'onglet **Filtre**.
4. Sélectionnez ou entrez le nom d'unité, le logiciel ou le nom d'utilisateur dans les zones correspondantes.
5. Cliquez sur **Filtrer**.

Vous pouvez sélectionner les informations utilisateur à afficher, éditer ou retirer.

### Edition des informations utilisateur dans l'outil de suivi des mots de passe
{: #cp_editusinfopwtracktool}

Après avoir ajouté un utilisateur, vous pouvez éditer les informations associées à l'utilisateur ou au mot de passe. Utilisez la procédure suivante pour éditer les informations d'un utilisateur dans l'outil de suivi des mots de passe.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez sur **Equipements** > **Gérer** > **Mots de passe** depuis le menu.
3. Localisez dans l'outil la combinaison appareil-utilisateur. Utilisez la fonction de filtre pour rapidement localiser un utilisateur.
4. Cliquez sur la ligne pour ouvrir la vue des détails de l'utilisateur.
5. Mettez à jour la zone **Nom d'utilisateur** ou **Mot de passe** selon vos besoins.
6. Cliquez sur **Mettre à jour** pour sauvegarder vos modifications.

Après qu'un utilisateur ou un mot de passe a été modifié dans l'outil de suivi des mots de passe, les informations sont immédiatement mises à jour.

## Configuration d'un compte pour un accès par mot de passe à usage unique
{: #cp_confportacc1timpwacc}

Avant de pouvoir configurer le compte, vous devez d'abord configurer l'application Verisign "VIP Access". Si vous n'avez pas encore configuré VIP Access, commencez par télécharger l'application pour l'un des appareils suivants :
* Pour votre téléphone : [https://m.vip.symantec.com/home.v ![Icône de lien externe](../icons/launch-glyph.svg)](https://m.vip.symantec.com/home.v){:new_window}
* Pour votre bureau : [https://idprotect.verisign.com/desktop/download.v ![Icône de lien externe](../icons/launch-glyph.svg)](https://idprotect.verisign.com/desktop/download.v){:new_window}

Procédez ensuite comme suit :
1. Ouvrez l'application. Accédez à vos données d'identification et à votre mot de passe à usage unique. Vous pouvez ignorer initialement le mot de passe, mais aurez besoin des données d'identification pour le portail ; conservez donc l'application ouverte.
2. Connectez-vous au portail client en tant qu'utilisateur pour lequel vous souhaitez configurer le mot de passe à usage unique.
3. Cliquez sur **Compte** > **Utilisateurs** > **Actions** > **Ajouter authentification externe**.
4. Sélectionnez le type d'authentification à ajouter. Si vous utilisez l'application Verisign, sélectionnez **Symantec Identity Protection**.
5. Entrez les données d'identification de l'étape 1 puis cliquez sur **Continuer**.
6. Exécutez le processus de commande et votre option de sécurité supplémentaire sera automatiquement appliquée en seulement quelques minutes.
7. Après plusieurs minutes, sélectionnez **Compte** > **Utilisateurs** dans la barre de navigation, puis sélectionnez l'utilisateur pour lequel vous avez configuré le mot de passe à usage unique.
8. Cliquez sur le lien **Mettre à jour l'accréditation** à la section **Paramètres de validation Symantec**.
9. Sélectionnez **activé** pour **Etat de l'accréditation** puis cliquez sur **Mettre à jour l'accréditation**.
10. Après que l'option de sécurité supplémentaire a été traitée, vous pouvez vous connecter au portail client comme à l'accoutumé. Une fois vos nom d'utilisateur et mot de passe soumis, vous êtes invité à entrer un code de sécurité.
11. Ouvrez l'application Verisign Identity Protection sur votre appareil préféré et indiquez le code affiché pour vous connecter.

Sauvegardez vos données d'identification Verisign Identity Protection d'origine dans un emplacement sécurisé pour un usage futur. Sans ces données, vous ne pourrez pas accéder au portail.

## Redéfinition de votre mot de passe
{: #cp_reset-your-password}

Le fait d'utiliser un IBMid pour la connexion à votre compte a des conséquences sur le mode de redéfinition de votre mot de passe.  

### Redéfinition d'un mot de passe de compte IBMid
{: #cp_reset-IBMid-password}

Si vous utilisez IBMid pour l'authentification, pour redéfinir ou récupérer votre mot de passe, accédez à votre profil IBMid et suivez les instructions sous la section d'**ouverture de connexion**.

### Redéfinition d'un mot de passe de compte
{: #cp_reset-password}

Si vous n'utilisez pas d'IBMid pour l'authentification de compte, procédez comme suit :

1. Cliquez sur le lien de mot de passe perdu sur la page de connexion du [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}.
2. Entrez votre nom d'utilisateur actuel.
3. Vérifiez dans votre messagerie si vous avez reçu un lien pour redéfinition du mot de passe. Ce lien reste valide pendant 24 heures.
4. Sélectionnez et répondez à trois questions de sécurité.

Vous disposez de cinq tentatives pour répondre aux questions de sécurité. Si vous dépassez ce nombre, le formulaire de réinitialisation du mot de passe est verrouillé pendant 15 minutes avant que vous ne puissiez faire une nouvelle tentative.

Pour plus d'informations sur l'utilisation des mots de passe VPN, voir [Mise à jour du mot de passe VPN d'un utilisateur ](/docs/infrastructure/iaas-vpn/update-password.html#update-a-user-s-vpn-password).
{: tip}
