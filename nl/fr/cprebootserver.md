---

copyright:

  years: 1994, 2018

lastupdated: "2017-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Réamorçage du serveur
{: #customerportal_rebootserver}

Des événements surviennent parfois au niveau de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} qui nécessitent de redémarrer le serveur.
{:shortdesc}

Utilisez les étapes suivantes pour redémarrer votre serveur :
1. Depuis le portail client, cliquez sur l'onglet **Support**.
2. Cliquez sur **reboot**.
3. Sélectionnez le serveur à redémarrer et cliquez sur **reboot**.
4. Sélectionnez l'une des méthodes suivantes pour redémarrer le serveur :
  * Par défaut (tente le redémarrage avec IPMI puis avec la multiprise)
  * IPMI
  * Multiprise
5. Cliquez sur **reboot**.

Cette page permet également un amorçage sur le noyau de secours, ce qui peut s'avérer particulièrement utile en cas d'incident, si le serveur ne parvient pas à amorcer sur le système d'exploitation à cause d'un problème de configuration. Après l'amorçage du serveur sur le noyau de secours, vous pouvez monter la ou les unités puis corriger le problème de configuration. Une fois le problème corrigé, vous pouvez redémarrer le serveur à partir de la ligne de commande et le serveur redémarre sur son noyau par défaut. Une fois la commande restart émise, une durée estimative d'achèvement de l'opération s'affiche.
