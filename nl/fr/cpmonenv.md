---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Surveillance de votre environnement et des événements système
{: #customerportal_cpmonenvsysevent}

La surveillance de votre environnement signifie que vous avez la possibilité de contrôler les appareils à tout moment et que vous êtes automatiquement notifié si l'un des équipements tombe en panne. Vous pouvez également surveiller les événements système afin de garantir un fonctionnement harmonieux.  
{: shortdesc}

## Surveillance de votre environnement
{: #cpmonenv}

Au minimum, utilisez la surveillance de base par commande ping. Vous avez néanmoins la possibilité de personnaliser vos options de surveillance de la façon la mieux adaptée à vos besoins métier.

### Etre tenu informé de la maintenance réseau et des événements imprévus
{: #cp_stayinfomaintevent}

De temps en temps, des opérations de maintenance réseau planifiées et urgentes sont inévitables. L'infrastructure {{site.data.keyword.BluSoftlayer_full}} gère de nombreux canaux afin de vous tenir informé de tous les événements de maintenance planifié et d'urgence. En outre, vous pouvez vous [abonner aux notifications par e-mail](/docs/customer-portal/cpsub2not.html) depuis le système de gestion d'événements. Ce service gratuit envoie automatiquement des courriers électroniques aux utilisateurs abonnés concernant les événements imprévus qui peuvent impacter des services.

### Utilisation du dispositif mobile de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}
{: #cp_bmxinframobile}

Utilisez le dispositif mobile de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour gérer les appareils de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} par mobile à l'aide de votre appareil iOS ou Android. La fonctionnalité au sein du dispositif mobile de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} inclut la prise en charge des demandes de service, le contrôle d'appareil de base et la surveillance de la bande passante.

L'application mobile de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} complète la fonctionnalité du portail client car elle vous permet de surveiller des informations essentielles sur votre infrastructure à partir de n'importe quel endroit à l'aide de votre périphérique mobile connecté au réseau. L'application évolue rapidement et de nouvelles fonctionnalités sont régulièrement ajoutées, mais vous pouvez utiliser l'application mobile pour effectuer des tâches comme les tâches suivantes :
  * Afficher, créer et mettre à jour des tickets de demande de service
  * Surveiller l'état des périphériques, y compris la bande passante et les alarmes
  * Arrêter et redémarrer des serveurs bare metal et des serveurs virtuels
  * Consulter les factures du compte et procéder à des paiements ponctuels
  * Accéder au contenu stocké dans Object Storage et l'examiner

L'application mobile de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} est disponible sur plusieurs plateformes de périphériques mobiles répandues et est disponible gratuitement à partir des magasins d'applications associés à chaque plateforme.

## Surveillance des serveurs
{: #customerportal_monservers}

Configurez la surveillance pour vérifier le statut de votre serveur et savoir quand vous devez le faire évoluer. Vous pouvez utiliser des services de surveillance standard ou Nimsoft. Vous pouvez employer la surveillance standard (de base) dans la méthode ping-avec-réponse en utilisant un ping avec réponse lente ou un ping de service à partir du portail client de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Vous pouvez également faire appel à la surveillance Nimsoft (avancée) à partir du portail client ou dans l'un des trois niveaux suivants : de base, avancé et premium. Pour plus d'informations sur les serveurs Bare Metal, voir [Initiation aux serveurs Bare Metal](/docs/bare-metal/about.html).

## Surveillance des événements système
{: #customerportal_monevent}

Vous pouvez surveiller les événements système en affichant les journaux d'audit et les journaux d'accès.

### Affichage d'un journal d'audit pour un compte
{: #cp_viewacctauditlog}

Chaque compte de portail client est fourni avec un journal d'audit qui assure le suivi des interactions de chaque utilisateur au sein du portail client. Par exemple, le suivi des interactions suivantes est effectué :
  * Tentatives de connexion (réussites et échecs)
  * Mises à jour de la vitesse de port
  * Mise sous tension ou hors tension et redémarrages
  * Interactions effectuées par le personnel d'assistance de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}.

Procédez comme suit pour afficher un journal d'audit pour un compte utilisateur.

1. Accédez au [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Gérer** > **Journal d'audit** depuis la barre de navigation afin d'accéder au journal d'audit.

Le journal d'audit affiche à l'origine les 25 dernières interactions effectuées sur le compte par des utilisateurs. Vous pouvez afficher jusqu'à 200 interactions à tout moment. Mettez à jour le nombre de résultats affichés depuis la liste déroulante **Affichage**. Si des paramètres ont été modifiés, la colonne **Action** de l'interaction comporte un lien. Cliquez sur un lien pour afficher le paramètre impacté par l'action et les détails du changement. Le fait de cliquer sur le nom de l'appareil ou sur le nom d'utilisateur pour une interaction vous redirige vers l'écran des détails de l'appareil ou l'écran du profil utilisateur.

### Affichage des journaux d'accès d'un utilisateur
{: #cp_viewuserlogs}

Les journaux d'accès affichent les données de chaque tentative d'accès effectuée par un utilisateur du portail client spécifique. Les journaux affichent une date et un horodatage, ainsi que l'adresse IP pour chaque tentative d'accès. Procédez comme suit pour afficher les journaux d'accès d'un utilisateur :

1. Accédez au [portail client ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} à l'aide de vos données d'identification uniques.
2. Sélectionnez **Compte** > **Utilisateurs** dans la barre de menus pour accéder à la fenêtre Utilisateurs.
3. Dans la liste déroulante **Actions**, sélectionnez **Afficher journal d'audit** pour afficher le journal d'accès de l'utilisateur.

Le journal d'accès de chaque utilisateur présente les tentatives d'accès effectuées par cet utilisateur par date, ainsi que l'adresse IP à partir de laquelle a eu lieu la tentative d'accès. Les informations du journal d'accès sont en lecture seule, il n'est donc pas possible d'éditer le contenu. Vous pouvez afficher les journaux d'audit à tout moment en répétant la procédure précédente. Pour quitter les journaux et revenir à l'écran Utilisateurs, cliquez sur le lien **Afficher tous les utilisateurs**.
