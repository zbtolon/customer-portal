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


# Effettuazione di un pagamento
{: #customerportal_makepayment}

Tutti i dettagli di fatturazione della tua infrastruttura {{site.data.keyword.Bluemix}}, dalle fatture alle informazioni di pagamento, vengono memorizzati in modo sicuro nel portale del cliente. Se il tuo metodo di pagamento cambia, o la tua carta di credito viene annullata o scade, aggiorna le informazioni di pagamento per evitare ritardi negli addebiti.
{:shortdesc}

## Visualizzazione della tua fattura
{: #cp_viewinvoice}

Nella finestra Fatture, ogni singola fattura viene riepilogata in base a numero di fattura, data, tipo di fattura e vari saldi monetari. Le fatture possono essere dei seguenti tipi:

<dl>
<dt>Nuovo</dt>
<dd>La prima fattura in una serie di fatture ricorrenti.</dd>
<dt>Ricorrente</dt>
<dd>Una fattura per gli addebiti ricorrenti che sono stati attivi sull'account per più di un mese.</dd>
<dt>Addebito una tantum</dt>
<dd>Un addebito una tantum per le varie spese, che potrebbero includere dei costi aggiuntivi.</dd>
<dt>Credito</dt>
<dd>Un credito dall'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} al saldo dell'account.</dd>
<dt>Rimborso</dt>
<dd>Un'inversione delle spese, per un addebito una tantum o ricorrente.</dd>
</dl>

Puoi anche visualizzare un riepilogo di fatturazione per l'account, incluso il saldo corrente e la stima del saldo successivo, il metodo di pagamento e le date dell'ultima e della prossima fattura ricorrente. 

1. Fai clic su **Account** > **Fatturazione** > **Fatture** dal menu.
2. Puoi anche visualizzare la fattura nel portale del cliente o scaricare la fattura.

Se visualizzi la fattura nel portale del cliente, viene mostrato un elenco dettagliato di voci di fatturazione per la fattura selezionata. Fai clic in qualsiasi punto della riga di una voce di fatturazione per visualizzare ulteriori dettagli relativi all'addebito. Se hai scaricato la fattura, puoi visualizzarla in base alle impostazioni del tuo browser. Le fatture scaricate forniscono sia un riepilogo dettagliato che una fatturazione dettagliata per ciascuna voce di fatturazione.

## Aggiunta di un metodo di pagamento
{: #cp_cpmanacctbillpay}

Ogni account SoftLayer è tenuto ad avere una carta di credito registrata in archivio su cui viene automaticamente addebitato l'importo della fattura ogni mese. Queste informazioni devono essere sempre aggiornate per evitare ritardi nei pagamenti; possono essere aggiornate in qualsiasi momento per garantire che le informazioni di pagamento siano sempre accurate. Se le informazioni della carta di credito registrate in archivio sono corrette ma deve essere applicata una forma alternativa di pagamento al saldo corrente, vedi [Effettuazione di un pagamento una tantum](/docs/customer-portal/cpmanacctbillpay.html#cp_makeonetimepayment). Utilizza la seguente procedura per aggiungere un metodo di pagamento per un account nel portale del cliente.

1. Fai clic su **Account** > **Fatturazione** > **Metodo di pagamento** dal menu.
2. Immetti i dettagli di fatturazione richiesti per la carta in ogni campo della sezione **Indirizzo di fatturazione**.
> **Nota:** fai clic sulla casella di spunta **Utilizza informazioni azienda** per completare automaticamente i campi in questa sezione con le informazioni sulla società che l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} ha in archivio per l'account.
3. Immetti le informazioni della carta di credito in ogni campo della sezione **Informazioni di pagamento**.
4. Fai clic su **Aggiungi carta di credito** per aggiungere la carta di credito come metodo di pagamento mensile. 
5. Facoltativamente, seleziona **Supportato UE** per assicurarti che il team di supporto in Europa gestisca i tuoi problemi di manutenzione e supporto.  Per ulteriori informazioni su questa opzione, vedi [Impostazione dell'opzione esclusiva del team di supporto europeo](/docs/customer-portal/pay-invoice.html#cp_seteusupported).

Dopo aver aggiunto il metodo di pagamento, la richiesta viene elaborata dai rappresentanti dell'account SoftLayer per garantire la validità della carta. Le carte convalidate sono disponibili per l'uso sull'account entro 24 ore. La modifica dello stato per il metodo di pagamento viene inviata via e-mail al contatto che è stato fornito quando è stato aggiunto il metodo di pagamento.

## Effettuazione di un pagamento una tantum
{: #cp_makeonetimepayment}

Puoi effettuare pagamenti una tantum utilizzando un account PayPal o una carta di credito principale e puoi effettuare pagamenti per un saldo completo o parziale. I dettagli del pagamento una tantum non vengono registrati per l'utilizzo futuro e non modificano i metodi di pagamento mensili correnti per l'account.

1. Vai alla pagina Effettua un pagamento una tantum nel portale del cliente.
 * Dal menu, vai a **Account** > **Effettua un pagamento**.
 * Dalla pagina Fatture, fai clic su **Paga saldo**.
2. Immetti l'importo di pagamento nel campo **Importo del pagamento**.
3. Se effettui il pagamento con PayPal, fai clic su **PayPal** e segui le istruzioni in PayPal per completare il pagamento. Non sono richieste ulteriori azioni. Se effettui il pagamento con una carta di credito, immetti il **Numero della carta, la Data di scadenza e il Codice di sicurezza** nei campi appropriati. 
4. Immetti le informazioni di fatturazione nei campi appropriati nella sezione **Indirizzo di fatturazione della carta di credito**.
5. Facoltativamente, seleziona **Supportato UE** per assicurarti che il team di supporto in Europa gestisca i tuoi problemi di manutenzione e supporto.  Per ulteriori informazioni su questa opzione, vedi [Impostazione dell'opzione esclusiva del team di supporto europeo](/docs/customer-portal/pay-invoice.html#cp_seteusupported).
6. Fai clic su **Paga con carta di credito** per avviare il pagamento.

Dopo aver avviato il pagamento, il pagamento viene elaborato di conseguenza. Se si verificano problemi con il pagamento, segui le istruzioni indicate dall'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} o da PayPal finché il problema non viene risolto. Il pagamento viene elaborato, l'importo viene applicato e il saldo corrente viene aggiornato..
