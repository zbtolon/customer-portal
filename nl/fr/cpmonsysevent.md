---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# Surveillance des événements système de l'infrastructure {{site.data.keyword.Bluemix_notm}}
{: #customerportal_monevent}

Vous pouvez surveiller les événements système pour que vos systèmes continuent à fonctionner de façon harmonieuse.  Pour des informations sur la configuration et la gestion de serveurs virtuels dans l'infrastructure {{site.data.keyword.BluSoftlayer_full}}, voir [Initiation aux serveurs virtuels](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers).
{:shortdesc}

## Affichage d'un journal d'audit pour un compte
{: #cp_viewacctauditlog}

Chaque compte de portail client est fourni avec un journal d'audit qui assure le suivi des interactions de chaque utilisateur au sein du portail client. Les interactions suivies incluent les tentatives de connexion (qu'elles aboutissent ou échouent), les mises à jour de vitesse de port, les mises sous ou hors tension et les réamorçages, ainsi que les interactions effectuées par l'équipe de support de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Procédez comme suit pour afficher un journal d'audit pour un compte utilisateur.

1. Accédez au [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Gérer** > **Journal d'audit** depuis la barre de navigation afin d'accéder au journal d'audit.

Le journal d'audit affiche à l'origine les 25 dernières interactions effectuées sur le compte par des utilisateurs. Vous pouvez afficher jusqu'à 200 interactions à tout moment. Mettez à jour le nombre de résultats affichés depuis la liste déroulante **Affichage**. Si des paramètres ont été modifiés, la colonne **Action** de l'interaction comportera un lien. Cliquez sur un lien pour afficher le paramètre impacté par l'action et les détails du changement. Le fait de cliquer sur le nom de l'appareil ou le nom d'utilisateur pour une interaction vous redirige respectivement vers l'écran des détails de l'unité ou l'écran du profil utilisateur.

## Affichage des journaux d'accès d'un utilisateur
{: #cp_viewuserlogs}

Les journaux d'accès affichent les données de chaque tentative d'accès effectuée par un utilisateur du portail client spécifique. Les journaux affichent une date et un horodatage, ainsi que l'adresse IP pour chaque tentative d'accès. Procédez comme suit pour afficher les journaux d'accès d'un utilisateur :

1. Accédez au [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Utilisateurs** dans la barre de menus pour accéder à la fenêtre Utilisateurs.
3. Dans la liste déroulante **Actions**, sélectionnez **Afficher journal d'audit** pour afficher le journal d'accès de l'utilisateur.

Le journal d'accès de chaque utilisateur montre les tentatives d'accès effectuées par cet utilisateur par date, ainsi que l'adresse IP à partir de laquelle a eu lieu la tentative d'accès. Les informations du journal d'accès sont en lecture seule, il n'est donc pas possible d'éditer le contenu. Vous pouvez afficher les journaux d'audit à tout moment en répétant la procédure précédente. Pour quitter les journaux et revenir à l'écran Utilisateurs, cliquez sur le lien **Afficher tous les utilisateurs** en haut de l'écran.
