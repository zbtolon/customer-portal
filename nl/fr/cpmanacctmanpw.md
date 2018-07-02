---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-22"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestion du suivi des mots de passe
{: #customerportal_manpws}

Si vous êtes utilisateur principal ou propriétaire d'un compte, vous pouvez activer le suivi des mots de passe, ainsi que configurer un mot de passe à usage unique pour le compte. Le suivi des mots de passe permet aux utilisateurs de stocker les données de mot de passe logiciel pour des appareils et leur logiciel associé.
{:shortdesc}

## Activation du suivi des mots de passe
{: #customerportal_enabpwtrak}

Le portail client comporte un outil facultatif de [suivi des mots de passe ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/devices/passwords){:new_window} pour chaque compte. Les utilisateurs peuvent récupérer leurs noms d'utilisateur et mots de passe via l'outil en cas de perte ou d'oubli de ces informations.

Les équipes de support utilisent également le suivi des mots de passe si l'accès distant à un système est requis. Les noms d'utilisateur et mots de passe sont utilisés par le support uniquement si nécessaire et autorisé pour la résolution de ticket.

Le suivi des mots de passe dans le portail client est facultatif. N'importe quel utilisateur disposant des droits appropriés peut voir tous les mots de passe stockés par cet outil. Les informations d'utilisateur et de mot de passe sont suivies manuellement de façon à ne pas être automatiquement synchronisées avec un appareil ou son logiciel. C'est pourquoi vous devez veiller à mettre à jour l'outil de suivi des mots de passe en même temps que vous mettez à jour les utilisateurs et les mots de passe sur l'appareil et le logiciel. Utilisez la procédure suivante pour ajouter un utilisateur à l'outil de suivi des mots de passe.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez sur **Equipements** > **Gérer** > **Mots de passe** depuis le menu.
3. Cliquez sur l'onglet **Ajouter identifiants**.
4. Sélectionnez le **Nom de l'unité** auquel l'utilisateur est associé depuis la liste déroulante **Nom de l'unité**.
5. Sélectionnez le **Logiciel** auquel l'utilisateur est associé depuis la liste **Logiciel**.

  Le logiciel répertorié est fourni par l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} via des abonnements payants ou gratuits. Aucun logiciel tiers installé manuellement sur l'appareil n'est disponible pour suivi via le portail client.
  {: tip}

6. Entrez le nom d'utilisateur et le mot de passe pour le logiciel dans les zones appropriées.
8. Facultatif : Vous pouvez entrer tout commentaire adéquate dans la zone **Remarques**.
9. Cliquez sur **Ajouter identifiants**.

Une fois l'utilisateur ajouté à l'outil de suivi des mots de passe, les informations sont stockées dans l'outil jusqu'à leur suppression manuelle. Par défaut, toutes les combinaisons de nom d'utilisateur et de mot de passe sont stockées en fonction du nom de l'appareil. Les entrées sont affichées par ordre alphabétique, par nom d'appareil puis par nom d'utilisateur.

### Filtrage des informations dans l'outil de suivi des mots de passe
{: #cp_filterusinfopwtracktool}

Pour afficher, éditer ou supprimer des informations utilisateur depuis l'outil de suivi des mots de passe, vous pouvez appliquer un filtre afin de rapidement localiser un utilisateur. Ce filtrage est pratique lorsque la liste des utilisateurs couvre de nombreuses lignes ou pages. Utilisez la procédure suivante pour filtrer par appareil, logiciel ou utilisateur dans l'outil de suivi des mots de passe.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez sur **Equipements** > **Gérer** > **Mots de passe** depuis le menu.
3. Cliquez sur l'onglet **Filtre**.
4. Sélectionnez ou entrez le nom d'unité, le logiciel ou le nom d'utilisateur dans les zones correspondantes.
5. Cliquez sur **Filtrer**.

Vous pouvez sélectionner les informations utilisateur à afficher, éditer ou retirer.

### Edition des informations utilisateur dans l'outil de suivi des mots de passe
{: #cp_editusinfopwtracktool}

Une fois qu'un utilisateur a été ajouté à l'outil de suivi des mots de passe, vous pouvez éditer les informations associées à l'utilisateur ou au mot de passe. Utilisez la procédure suivante pour éditer les informations d'un utilisateur dans l'outil de suivi des mots de passe.

1. Accédez au portail client à l'aide de vos données d'identification uniques.
2. Cliquez sur **Equipements** > **Gérer** > **Mots de passe** depuis le menu.
3. Localisez dans l'outil la combinaison appareil-utilisateur. Utilisez la fonction de filtre pour rapidement localiser un utilisateur.
4. Cliquez sur la ligne pour ouvrir la vue des détails de l'utilisateur.
5. Mettez à jour la zone **Nom d'utilisateur** ou **Mot de passe** selon les besoins.
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
4. Sélectionnez le type d'authentification à ajouter. Si vous utilisez l'application Verisign, choisissez **Symantec Identity Protection**.
5. Entrez les données d'identification de l'étape 1 puis cliquez sur **Continuer**.
6. Exécutez le processus de commande et votre option de sécurité supplémentaire sera automatiquement appliquée en seulement quelques minutes.
7. Après plusieurs minutes, sélectionnez **Compte** > **Utilisateurs** dans la barre de navigation, puis sélectionnez l'utilisateur pour lequel vous avez configuré le mot de passe à usage unique.
8. Cliquez sur le lien **Mettre à jour l'accréditation** à la section **Paramètres de validation Symantec**.
9. Sélectionnez **activé** pour **Etat de l'accréditation** puis cliquez sur **Mettre à jour l'accréditation**.
10. Après que l'option de sécurité supplémentaire a été traitée, vous pouvez vous connecter au portail client comme à l'accoutumé. Une fois vos nom d'utilisateur et mot de passe soumis, vous êtes invité à entrer un code de sécurité.
11. Ouvrez l'application Verisign Identity Protection sur votre appareil préféré et indiquez le code affiché pour vous connecter.

Sauvegardez vos données d'identification Verisign Identity Protection d'origine dans un emplacement sécurisé pour un usage futur. Sans ces données, vous ne pourrez pas accéder au portail.
