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


# Protection de vos systèmes
{: #customerportal_protsys}

La protection de vos systèmes garantit leur bonne exécution, sans interruptions inutiles.

## Utilisez le réseau privé
{: #cp_bpuseprivnet}

Vous pouvez gérer vos appareils dans l'environnement le plus sécurisé possible à l'aide du réseau privé de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Lorsque cela est possible, interagissez avec vos unités à l'aide d'une connexion VPN et activez le spanning réseau afin que vos systèmes communiquent via le réseau privé. Pour accéder au réseau privé, éditez l'accès VPN de l'utilisateur depuis la [Liste utilisateurs ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Utilisez la liste [Virtual Private Network ![Icône de lien externe](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} pour vous connecter à l'une des options VPN.

Pour plus d'informations sur l'utilisation d'une connexion VPN, voir [A propos de la connexion VPN](/docs/infrastructure/iaas-vpn/about-vpn.html).

### Ne laissez pas de port RDP, SSH ou de contrôle sur le réseau public
{: #cp_bpnordpsshcponpubnet}

Le réseau public est parfait pour de nombreuses raisons, mais certains éléments, lorsqu'ils sont disponibles sur le réseau public via des ports ouverts, peuvent rendre votre système vulnérable. Protégez-vous en désactivant RDP ou en limitant SSH sur le réseau public. Si ces services doivent être disponibles sur le réseau public, envisagez de déplacer RDP ou SSH vers un numéro de port personnalisé.

## Protégez vos données via des sauvegardes régulières
{: #cp_bpsafedataregback}

Planifiez des sauvegardes pour vous assurer que vos données sont stockées en toute sécurité en dehors de votre unité afin de pouvoir les recharger en cas de perte.

L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} offre de nombreuses solutions de sauvegarde afin de garantir que vous pourrez récupérer vos données en cas de défaillance d'unité ou d'erreur d'un utilisateur. Les solutions de sauvegarde incluent NAS, EVault Backup et R1Soft CDP, qui sont tous disponibles dans différentes options de stockage.
Par exemple, vous pouvez choisir l'un des services de sauvegarde suivants pour stocker vos données dans un emplacement sécurisé :
  * EVault Backup est un système de sauvegarde automatique basé sur un agent. Il s'agit d'une solution simple et transparente de gestion de votre terminal. Il est compatible avec les logiciels Microsoft, y compris Exchange et SQL via des plug-in supplémentaires. Les utilisateurs d'EVault interagissent avec ce service via l'application Web WebCC d'EVault.
  * R1Soft Continuous Data Protection (CDP) peut être installé sur votre serveur ou sur une machine virtuelle auto-gérée. Il est recommandé si vous souhaitez disposer d'une seule interface pour gérer toutes vos sauvegardes. Vous interagissez avec R1Soft CDP via votre système de gestion propriétaire qui permet d'installer des agents sur des machines virtuelles et offre des plug-in de base de données pour plus de fonctionnalité.

 Consultez la page sur le [stockage ![Icône de lien externe](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} pour obtenir plus d'informations sur les différentes solutions de sauvegarde et consultez la rubrique [Initiation aux services de sauvegarde](/docs/infrastructure/Backup/index.html) pour obtenir plus d'informations sur la sauvegarde de vos données.

### Ne partez pas du principe que vous disposez d'une redondance, soyez-en sûr
{: #cp_bpknowredundant}

L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} offre plusieurs solutions de redondance sous forme de module complémentaire, notamment des chemins d'accès doubles, des alimentations redondantes et des configurations RAID. Vérifiez que vous disposez d'une ou de plusieurs de ces fonctions afin de garantir que vous travaillez dans un environnement redondant et êtes protégé en cas de panne.

### Assurez-vous que vos informations sont sauvegardées avant d'exécuter un rechargement du système d'exploitation
{: #cp_bpnoperfOSwobackupconf}

Le rechargement de votre système d'exploitation supprime toutes les données du disque dur de l'unité. Avant de lancer le rechargement du système d'exploitation, sauvegardez vos informations et vérifiez que la sauvegarde a abouti et qu'aucune donnée n'a été perdue. Une fois le rechargement du système d'exploitation terminé, il n'est plus possible de récupérer des informations.

## Ne supprimez pas Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} utilise ASM pour surveiller le statut de votre grappe RAID. Si vous supprimez ce logiciel, l'équipe de support ne peut pas surveiller votre unité. Si ASM est supprimé de votre unité, les alertes de défaillance RAID sur celle-ci ne sont pas disponibles et vous n'êtes pas notifié de la défaillance via le système de notification automatique.
