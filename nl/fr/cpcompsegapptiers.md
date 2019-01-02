---

copyright:

  years: 1994, 2018

lastupdated: "2018-10-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Sécurisation et évolutivité de votre environnement
{: #cp_compsegapptierssecscal}

Lorsque vous hébergez une application, deux des aspects les plus critiques à prendre en compte pour tout administrateur système sont la sécurité et l'évolutivité de l'application.
{:shortdesc}

## Sécurisation de vos systèmes avec des pare-feux
{: #cp_bpsecuresystem}

Utilisez les pare-feux matériels disponibles pour vous assurer que votre appareil est sécurisé en permanence. Vous pouvez mettre à disposition des pare-feux matériels à la demande sans temps d'indisponibilité si des règles sont correctement établies afin de protéger votre serveur contre toute activité indésirable.

Les pare-feux sont des services complémentaires à ajouter à tout appareil. Pour s'assurer de leur efficacité, il est nécessaire de les configurer et de les activer manuellement. Vous pouvez verrouiller les ports superflus et désactiver les ports publics pour des systèmes basés sur un réseau privé afin de gérer au plus près l'accessibilité externe à vos systèmes. L'exécution d'analyses de vulnérabilité régulières sur le portail client identifie les risques de sécurité en suspens ou inconnus afin de vous permettre de rapidement atténuer ces risques.

Après avoir commandé votre pare-feu, vous devez l'activer et définir des règles.

### Activation de votre pare-feu
{: #cp_bpnofirewalbypass}

L'achat d'un pare-feu constitue une première étape dans la protection de vos systèmes, mais se contenter d'acheter un pare-feu ne vous protégera pas. Une fois votre pare-feu mis à disposition, il se trouve en **mode contournement** et ne comporte aucune règle définie. Pour que votre pare-feu soit opérationnel, vous devez créer des règles et activer le pare-feu afin qu'il commence à bloquer tout activité indésirable.


## Sécurisation de votre environnement par segmentation de vos groupes de serveurs d'application
{: #cp_copmsecenv}

En segmentant vos groupes de serveurs d'application logiques en niveaux d'infrastructure physique, vous pouvez fournir un plus grand niveau de sécurité via l'utilisation de listes de contrôle d'accès (ACL). Lorsque vous segmentez vos groupes de serveurs d'applications, l'un des composants les plus critiques à prendre en compte est le trafic que vous autorisez à chaque niveau et depuis quelle origine. Pour déterminer ce point, réfléchissez à la façon dont votre application fonctionne à la base, et déterminez les services qui sont basés les uns sur les autres afin de fournir aux utilisateurs le contenu demandé.

Par exemple, avec une application à deux niveaux reposant sur un front end Web et un back end de base de données, vous aurez besoin de vous assurer que les ports 80 et 443 (si vous utilisez SSL) sont ouverts à Internet sur vos serveurs Web. Vous pouvez également verrouiller tous les ports Internet et gérer votre serveur par réseau privé virtuel (VPN) en utilisant le réseau privé de l'infrastructure {{site.data.keyword.BluSoftlayer_full}}, déconnecter l'adresse IP publique sur votre serveur de base de données et faire passer tout le trafic vers ce serveur via le port 1433 (pour MSSQL) ou le port 3306 (pour {{site.data.keyword.mysql}}) depuis votre serveur Web et gérer votre serveur de base de données via le réseau privé tout comme votre serveur Web. Pour finir, vous pouvez configurer un pare-feu logiciel sur le serveur de base de données afin de verrouiller tout le trafic depuis le serveur Web sur des ports de base de données spécifiques.

En configurant votre environnement de cette façon, vous augmentez le niveau de sécurité en empêchant l'accès à SSH ou RDP depuis Internet et en désactivant la totalité du trafic Internet vers votre base de données. La création de listes de contrôle d'accès entre la couche Web et la couche de base de données rend plus difficile la compromission de votre base de données si votre serveur Web venait à être compromis.

## Mise à l'échelle de votre environnement par la segmentation de vos groupes de serveurs d'application
{: #cp_copmscaleenv}

Un environnement multiniveau offre également une simplicité d'évolutivité comparativement à des architectures verticales ou à hôte unique. Vous pouvez configurer un environnement multiniveau pour faciliter l'évolutivité de votre application en autorisant l'adaptation des services ayant besoin de ressources supplémentaires. Par exemple, dans le scénario précédent, si votre serveur Web est sursollicité, il vous suffit de déployer un autre serveur Web. Vous pouvez ensuite répliquer le site ou les données d'application et équilibrer la charge ou configurer un serveur DNS round robin pour activer vos deux serveurs Web de façon à fractionner votre charge Web. Le serveur DNS round robin ou l'équilibrage de charge fournit une haute disponibilité à votre environnement en activant plusieurs serveurs Web pour répondre aux demandes entrantes. Si un seul serveur tombe en panne, un autre noeud est disponible pour gérer les demandes d'utilisateur.

Vous pouvez également ajuster votre base de données. Par exemple, avec une base de données {{site.data.keyword.mysql}}, une option consiste à configurer un autre serveur physique et à l'utiliser comme subordonné dans une configuration de réplication {{site.data.keyword.mysql}}. Vous pouvez segmenter toutes les opérations d'écriture de votre base de données sur le maître et toutes les opérations de lecture sur un ou plusieurs subordonnés afin de mettre à l'échelle la base de données de façon à supporter davantage de charge. Ce type de configuration permet également d'ajouter un niveau de haute disponibilité car vous pouvez changer le statut d'un subordonné en maître. Vous pouvez ensuite acheminer le trafic de lecture et d'écriture vers le subordonné si votre noeud maître {{site.data.keyword.mysql}} tombe en panne.

Ces idées ne représentent que quelques-unes des nombreuses façons de sécuriser et mettre à l'échelle votre environnement. Si vous avez des questions ou des doutes liés à la façon optimale de concevoir votre environnement d'un point de vue sécurité ou évolutivité, une équipe d'ingénierie de vente dédiée à l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} peut vous aider.
