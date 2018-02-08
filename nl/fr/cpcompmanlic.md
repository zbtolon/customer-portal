---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-06"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Gestion des équipements
{: #cp_compacclisc}

Vous pouvez gérer les licences du logiciel de panneau de commande actif, comme cPanel et Parallels, depuis le portail client, dans la fenêtre Licences du panneau de configuration. Vous pouvez afficher des licences et leurs IP associées, télécharger des fichiers de licence et annuler des licences individuelles. Vous pouvez également gérer les mots de passe du logiciel sur chaque appareil, depuis le portail client.
{:shortdesc}


## Téléchargement d'une licence sur un appareil
{: #cp_compdllisc}

Un fichier de licence est utilisé pour vérifier que la licence est valide pour le logiciel sur un appareil, ainsi que toute fonction logicielle activée. Vous pouvez télécharger des fichiers de licence depuis le portail client, mais uniquement sur l'appareil qui exécute le logiciel de panneau de commande correspondant. Utilisez la procédure suivante pour télécharger un fichier de licence.

1. Connectez-vous au portail client à l'aide de vos données d'identification uniques.
2. Sélectionnez **Equipements** > **Gérer** > **Licences du panneau de configuration** depuis le menu pour accéder à la fenêtre Licences du panneau de configuration.
3. Pour la licence, sélectionnez **Actions > Télécharger le fichier de licence**.
4. Sauvegardez ou téléchargez le fichier du logiciel du panneau de commande sur l'appareil à l'aide des invites fournies par le système d'exploitation de l'appareil.

Après que vous avez téléchargé le fichier de licence sur l'appareil, les détails du logiciel du panneau de commande concernant la licence sont mis à jour. Si des problèmes surviennent, ou si le téléchargement n'aboutit pas, relancez le processus de téléchargement en répétant les étapes précédentes.

## Annulation d'une licence de panneau de configuration
{: #cp_compcanlisc}

Les licences de panneau de configuration sont facturées sur une base mensuelle, en fonction des dispositions acceptées au moment de l'achat de la licence. Vous pouvez annuler des licences à tout moment, et elles seront annulées à la prochaine date anniversaire de facturation suivante. Pour s'assurer qu'une annulation est correctement appliquée au cycle de facturation en cours, elle doit être faite au moins 24 heures avant la date anniversaire de facturation. Des informations spécifiques sur la date anniversaire de facturation pour le compte seront affichées durant le processus d'annulation. Utilisez la procédure suivante pour annuler une licence de panneau de configuration.

1. Effectuez une sauvegarde ou transférez les données associées à la licence.
2. Connectez-vous au portail client à l'aide de vos données d'identification uniques.
3. Sélectionnez **Equipements** > **Gérer** > **Licences du panneau de configuration** depuis le menu pour accéder à la fenêtre Licences du panneau de configuration.
4. Sélectionnez **Actions** > **Annuler** pour la licence de panneau de configuration à annuler.
5. Entrez des remarques concernant l'annulation dans la zone de texte **Remarques**.
6. Cliquez sur **Continuer** pour passer à l'écran de confirmation.
7. Sélectionnez la case à cocher d'**accusé de réception de perte de données**.

  Si vous n'avez pas sauvegardé des données importantes, revenez à la première étape et sauvegardez toutes les données avant d'annuler la licence.
  {: tip}

8. Cliquez sur **Annuler la licence**.

Après que vous avez initié le processus d'annulation, la licence de panneau de configuration est planifiée pour être annulée à la date anniversaire de facturation à venir. Si l'annulation a été faite par erreur, vous pouvez l'annuler depuis l'écran Annulation du portail client.

## Gestion des mots de passe logiciels sur des appareils
{: #cp_bpmanacctresp}

A chaque composant logiciel mis à disposition sur un appareil est affecté un mot de passe généré automatiquement par les systèmes de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Les mots de passe logiciels pour chaque appareil sont stockés dans l'onglet **Mots de passe** de l'écran Détails de l'unité du portail client. Lorsque vous accédez au logiciel pour la première fois, changez vos mots de passe. Vous avez également la possibilité de stocker des données d'identification logicielles dans l'onglet **Mots de passe** de chaque appareil. Cependant, lorsque vous stockez des mots de passe sur le portail client, toute personne disposant d'un accès au compte et des droits appropriés peut consulter ces mots de passe.
