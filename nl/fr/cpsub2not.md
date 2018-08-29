---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-23"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Abonnement aux notifications
{: #cp_bpnotifications}

Parfois, des événements se produisent dans l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} qui nécessitent une action ; certains sont inattendus et d'autres correspondent à des activités de maintenance planifiée requises pour conserver l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} à ses conditions optimales de fonctionnement. Les clients sont isolés au maximum de ces événements, mais il est parfois nécessaire de déconnecter l'équipement. Quel que soit l'impact au niveau des clients, il faut toujours être transparent, respecter les délais et fournir les informations.
{:shortdesc}

Parce que vous devez rester maître de votre expérience cloud, vous avez besoin d'informations en temps utile sur les activités de maintenance. Pour obtenir ces informations, vous pouvez vous abonner aux notifications du portail client. L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} utilise le processus de notification EMS (système de gestion d'événements) pour les types suivants d'événements opérationnels importants :
* Problèmes d'infrastructure imprévus : Problèmes pouvant causer une indisponibilité sous certaines conditions pour des clients spécifiques
* Evénements de maintenance planifiée : Maintenance requise pour conserver le fonctionnement de l'infrastructure à un niveau optimal
* Tickets de demande de service ouverts : Alerte les utilisateurs abonnés des tickets ouverts sur leur compte

Les notifications de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} ont été conçues pour des environnements cloud en adhérant aux principes clé suivants :
* Automatisation via le portail client
* Evolutivité pour atteindre une communauté importante et grandissante
* Activation ciblée de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} afin d'identifier les seuls clients et sous-réseaux de ressources affectés par l'événement

Pour que le système de notification soit pleinement efficace, abonnez-vous au processus. Si vous possédez un environnement critique qui le nécessite, établissez également une couverture 24/24.

Pour une présentation de la façon dont les notifications de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} sont fournies, voir [Improving communications for customer-affecting planned events ![Icône de lien externe](../icons/launch-glyph.svg)](http://blog.softlayer.com/2014/improving-communications-customer-affecting-planned-events){:new_window}.

## Principes de diffusion des notifications
{: #cp_bpgsnotiftimpol}

L'avance avec laquelle l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} indique aux utilisateurs un événement en attente varie selon que l'événement est un problème d'infrastructure imprévu ou une opération de maintenance planifiée. En règle générale, la politique de infrastructure {{site.data.keyword.BluSoftlayer_notm}} consiste à remédier au problème aussi rapidement que possible afin de supprimer ou de réduire le risque de voir des problèmes supplémentaires se développer qui pourraient avoir un impact plus large. En d'autres termes, il arrive parfois qu'une maintenance planifiée soit effectuée en ayant été notifiée très peu de temps auparavant.

### Présentation des règles
{: #cp_bpgsnotifpolover}

Vous êtes notifiés des types d'indisponibilité ou de problème suivants comme décrit à chaque section.

#### Indisponibilités ou problèmes imprévus
L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} communique avec les clients concernés aussi rapidement que possible en fournissant des informations relatives à la portée de l'infrastructure, aux solutions palliatives ou aux estimations de résolution dès que ces informations sont connues. Une communication dans les plus brefs délais vous donne les informations nécessaires pour prévoir les contingences et offre l'assurance que l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} traite le problème.

#### Maintenance planifiée
L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} fournit à l'avance une notification pour la maintenance planifiée. Il peut arriver que la maintenance de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} soit urgente, ce qui peut entraîner une notification peut de temps avant l'événement. L'objectif est de trouver l'équilibre idéal entre la fourniture d'un préavis raisonnable pour vous permettre de planifier les contingences et la mise à niveau ou l'amélioration de l'infrastructure qui, généralement, se traduit par des améliorations apportées à la stabilité globale ou l'ajout de nouvelles fonctions.

#### Vulnérabilités en matière de sécurité
L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} isole la zone concernée, crée un correctif pour traiter cette vulnérabilité et teste le correctif afin de s'assurer qu'aucune fonction collatérale n'est impactée. Souvent, ce travail est effectué par un autre fournisseur qui peut fournir des composants de la technologie affectée. Il existe généralement un embargo sur les notifications publiques, qui ne sont envoyées que peu de temps avant pour des raisons de protection, mais ce mode de fonctionnement implique une période de notification plus courte. L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} implémente les correctifs sur l'infrastructure concernée avant que le public n'aie connaissance du problème, afin d'éviter d'augmenter les risques. Plus la vulnérabilité est traitée rapidement, plus vite le risque disparaît, ce qui signifie que les problèmes de sécurité requièrent une fenêtre de notification brève.

L'une des cibles les plus fréquentes des violations de sécurité est le logiciel d'infrastructure virtuelle. L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} utilise une technologie en partenariat et open source répandue afin de distribuer son offre de serveur virtuel. Pour implémenter un correctif de sécurité, il se peut que les serveurs client exécutant le logiciel d'infrastructure virtuelle doivent être mis hors ligne pour appliquer le correctif et réamorcer l'environnement, ce qui provoque une interruption. Afin de minimiser l'impact chez les clients, l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} a récemment mis en oeuvre une amélioration du processus de notification pour l'infrastructure virtuelle : les communications améliorées. Les clients sont notifiés d'une heure de début spécifique et d'une fenêtre de 90 minutes pour chaque pod, ce qui se traduit par un temps d'interruption plus court et un timing plus précis pour vous aider à mieux vous préparer. Le système de notification isole la maintenance sur chaque compte, ce qui permet à l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} de notifier les clients dès que leurs hôtes spécifiques passent en maintenance, ce qui se produit souvent bien avant la fenêtre de 90 minutes.

#### Plusieurs POD ou centres de données affectés
L'infrastructure {{site.data.keyword.BluSoftlayer_notm}} s'efforce de fournir un préavis plus important, hormis en cas d'extrême urgence nécessitant d'implémenter le correctif afin d'éviter un impact secondaire encore plus grand.


## Ajout d'abonnés aux notifications d'événements
{: #cp_bpaddsub2eventnotcp}

Les clients IBM comptent de plus en plus sur les services de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} (IaaS), que ce soient par des contrats avec IBM pour des services d'infrastructure gérés qui s'exécutent sur l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} ou par des contrats passés directement avec des services de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. Lorsque des services cloud impliquent l'infrastructure, seuls les utilisateurs de compte SoftLayer sont autorisés à recevoir des notifications, comme décrit à la section précédente. Dans certains cas, il se peut que vous n'ayez pas besoin des équipes de service géré ou de compte IBM impliquées dans les opérations de support des services d'infrastructure pour accéder à vos comptes SoftLayer. Une nouvelle fonction a été ajoutée au portail client de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} pour vous permettre de désigner une liste d'abonnés, comme du personnel IBM, pour recevoir les notifications sans disposer de droits sur vos comptes.

Pour désigner une liste d'abonnés, les utilisateurs principaux peuvent se connecter à leur compte de portail client  et utiliser la procédure suivante :
1. Cliquez sur **Support** > **Evénements** dans le menu.
2. Choisissez le type d'événement auquel ajouter des abonnés.
2. Depuis la fenêtre contextuelle, ajoutez la ou les adresses e-mail. Il peut s'agir d'adresses IBM ou non.
3. Cliquez sur **Créer**.

Les adresses e-mail ajoutées en tant qu'abonnés supplémentaires reçoivent les notifications d'événement planifié et non planifié, ainsi que les tickets de demande de service ouverts. Les notifications contiennent des détails techniques à prendre en compte lors de l'ajout d'abonnés. En raison de la nature technique des informations détaillées des notifications, les abonnés visés sont ceux qui peuvent comprendre, en détail, comment la notification va impacter environnement d'infrastructure {{site.data.keyword.BluSoftlayer_notm}}. L'abonnement de destinataires qui ne seraient pas à même de comprendre l'impact client potentiel en fonction des détails des notifications est contre-productif et il est fortement recommandé de ne pas les abonner.
