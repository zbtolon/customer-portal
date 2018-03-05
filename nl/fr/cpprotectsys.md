---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-04"

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

Vous pouvez gérer vos appareils dans l'environnement le plus sécurisé possible à l'aide du réseau privé de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Lorsque cela est possible, interagissez avec vos unités à l'aide d'une connexion VPN et activez le spanning réseau afin que vos systèmes communiquent via le réseau privé. Pour accéder au réseau privé, éditez l'accès VPN de l'utilisateur depuis la [Liste utilisateurs ![Icône de lien externe](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Utilisez les instructions de [Réseau privé virtuel ![Icône de lien externe](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} pour vous connecter à l'une des différentes options de VPN.

### Ne laissez pas de port RDP, SSH ou de contrôle sur le réseau public
{: #cp_bpnordpsshcponpubnet}

Le réseau public est parfait pour de nombreuses raisons, mais certains éléments, lorsqu'ils sont disponibles sur le réseau public via des ports ouverts, peuvent rendre votre système vulnérable. Protégez-vous en désactivant RDP ou en limitant SSH sur le réseau public. Si ces services doivent être disponibles sur le réseau public, envisagez de déplacer RDP ou SSH vers un numéro de port personnalisé.

## Protégez vos données via des sauvegardes régulières
{: #cp_bpsafedataregback}

L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} offre de nombreuses solutions de sauvegarde afin de garantir que vous pourrez récupérer vos données en cas de défaillance d'unité ou d'erreur d'un utilisateur. Les solutions de sauvegarde incluent NAS, EVault Backup et R1Soft CDP, qui sont tous disponibles dans différentes options de stockage. Consultez la page sur le [stockage ![Icône de lien externe](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} pour plus d'informations sur les différentes solutions de sauvegarde.

### Ne partez pas du principe que vous disposez d'une redondance, soyez-en sûr
{: #cp_bpknowredundant}

L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} offre plusieurs solutions de redondance sous forme de module complémentaire, notamment des chemins d'accès doubles, des alimentations redondantes et des configurations RAID. Vérifiez que vous disposez d'une ou de plusieurs de ces fonctions afin de garantir que vous travaillez dans un environnement redondant et êtes protégé en cas de panne.

### Assurez-vous que vos informations sont sauvegardées avant d'exécuter un rechargement du système d'exploitation
{: #cp_bpnoperfOSwobackupconf}

Le rechargement de votre système d'exploitation supprime toutes les données du disque dur de l'unité. Avant de lancer le rechargement du système d'exploitation, sauvegardez vos informations et vérifiez que la sauvegarde a abouti et qu'aucune donnée n'a été perdue. Une fois le rechargement du système d'exploitation terminé, il n'est plus possible de récupérer des informations.

## Ne supprimez pas Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} utilise ASM pour surveiller le statut de votre grappe RAID. Si vous supprimez ce logiciel, l'équipe de support ne peut pas surveiller votre unité. Si ASM est supprimé de votre unité, les alertes de défaillance RAID sur celle-ci ne sont pas disponibles et vous n'êtes pas notifié de la défaillance via le système de notification automatique.
