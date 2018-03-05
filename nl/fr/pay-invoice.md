---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-07"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Paiement
{: #customerportal_makepayment}

Tous les détails de facturation de votre infrastructure {{site.data.keyword.Bluemix}}, depuis les factures jusqu'aux informations de paiement, sont stockés de manière sécurisée sur le portail client. Si votre mode de règlement change, ou si votre carte de crédit est annulée ou arrive à expiration, mettez à jour vos informations de paiement afin d'éviter des frais ultérieurs.
{:shortdesc}

## Affichage de votre facture
{: #cp_viewinvoice}

Dans la fenêtre Factures, chaque facture individuelle est récapitulé par numéro de facture, date, type de facture, ainsi que divers soldes monétaires. Les factures peuvent être de l'un des types suivants :

<dl>
<dt>Nouveau</dt>
<dd>Première facture d'une série de factures récurrentes.</dd>
<dt>Récurrent</dt>
<dd>Facture de frais périodiques actifs sur le compte pour plusieurs mois.</dd>
<dt>Frais ponctuels</dt>
<dd>Frais uniques correspondant à diverses dépenses et pouvant inclure des dépassements.</dd>
<dt>Crédit</dt>
<dd>Crédit de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} dans le solde du compte.</dd>
<dt>Remboursement</dt>
<dd>Remboursement de frais, qu'ils soient ponctuels ou périodiques.</dd>
</dl>

Vous pouvez également afficher un récapitulatif de facturation pour le compte, incluant le solde en cours et le solde estimé suivant, le mode de règlement, ainsi que les dates des factures récurrentes précédente et suivante.

1. Cliquez sur **Compte** > **Facturation** > **Factures** dans le menu.
2. Vous pouvez afficher une facture dans le portail client ou la télécharger.

Si vous affichez la facture dans le portail client, une liste détaillée des éléments de facturation s'affiche pour la facture sélectionnée. Cliquez sur la ligne d'un élément de facturation pour afficher des détails supplémentaires concernant les frais. Si vous avez téléchargé la facture, vous pouvez l'afficher en fonction des paramètres de votre navigateur. Les factures téléchargées fournissent un récapitulatif détaillé ainsi que des détails pour chaque élément de facturation.

## Ajout d'un mode de règlement
{: #cp_cpmanacctbillpay}

Chaque compte SoftLayer doit comporter une carte de crédit enregistrée sur laquelle est automatiquement prélevé chaque mois le montant facturé. Ces informations doivent toujours être à jour afin d'éviter des pénalités de retard ; elles peuvent être mises à jour à tout moment afin de garantir des informations toujours exactes. Si les informations de carte de crédit enregistrées sont correctes mais qu'une autre forme de paiement doit être appliquée au solde en cours, voir comment [effectuer un règlement ponctuel](/docs/customer-portal/cpmanacctbillpay.html#cp_makeonetimepayment). Utilisez la procédure suivante pour ajouter un mode de règlement pour un compte dans le portail client.

1. Cliquez sur **Compte** > **Facturation** > **Mode de règlement** depuis le menu.
2. Entrez dans chaque zone les détails de facturation requis pour la carte à la section **Adresse de facturation**.
> **Remarque :** Cochez la case **Utiliser les informations de la société** pour renseigner automatiquement les zones de cette section à l'aide des informations de la société que l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} a enregistrées pour le compte.
3. Entrez les informations de carte de crédit dans chaque zone de la section **Informations de paiement**.
4. Cliquez sur **Ajouter carte de crédit** pour ajouter la carte de crédit en tant que mode de règlement mensuel.
5. Facultatif : Sélectionnez **Support dans l'Union européenne** pour vous assurer que l'équipe de support en Europe gère vos problèmes de maintenance et de support.  Pour plus d'informations sur cette option, voir la rubrique permettant de [définir l'option d'équipe de support exclusivement européenne](/docs/customer-portal/pay-invoice.html#cp_seteusupported).

Une fois le mode de règlement ajouté, la demande est traitée par les représentants de compte SoftLayer afin de garantir la validité de la carte. Les cartes validées sont disponibles pour utilisation sur le compte sous 24 heures. Le changement de statut du mode de règlement est envoyé par e-mail au contact fourni lors de l'ajout du mode de règlement.

## Exécution d'un règlement unique
{: #cp_makeonetimepayment}

Vous pouvez effectuer des paiements ponctuels à l'aide d'un compte PayPal ou d'une carte de crédit principale, et vous pouvez effectuer des paiements pour un solde partiel ou complet. Les détails du règlement unique ne sont pas enregistrés pour un usage futur et ne modifient pas les modes de règlement mensuel en cours pour le compte.

1. Accédez à la page Effectuer un règlement unique du portail client.
 * Depuis le menu : Accédez à **Compte** > **Effectuer un règlement**.
 * Depuis la page Factures : Cliquez sur **Régler solde**.
2. Entrez le montant du règlement dans la zone **Montant du Règlement**.
3. Si vous effectuez votre règlement via PayPal, cliquez sur **PayPal** et suivez les invites PayPal pour procéder au paiement. Aucune autre action n'est requise. Si vous effectuez votre règlement avec une carte de crédit, entrez les **numéro de carte, date d'expiration et code de sécurité** dans les zones appropriées.
4. Entrez les informations de de facturation dans les zones appropriées de la section **Adresse de facturation de la carte de crédit**.
5. Facultatif : Sélectionnez **Support dans l'Union européenne** pour vous assurer que l'équipe de support en Europe gère vos problèmes de maintenance et de support.  Pour plus d'informations sur cette option, voir la rubrique permettant de [définir l'option d'équipe de support exclusivement européenne](/docs/customer-portal/pay-invoice.html#cp_seteusupported).
6. Cliquez sur **Payer avec la carte de crédit** pour initier le paiement.

Une fois le règlement initié, celui-ci est traité en conséquence. En cas de problème au niveau du paiement, suivez les invites de l'infrastructure {{site.data.keyword.BluSoftlayer_notm}} ou de PayPal jusqu'à résolution du problème. Le paiement est traité, le montant est appliqué et le solde en cours est mis à jour.
