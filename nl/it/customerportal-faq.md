---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-07"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# FAQ
{: #bicpfaq}

Le seguenti domande frequenti riguardano la gestione dei problemi relativi alle risorse dell'infrastruttura.
{:shortdesc}


## Come posso recuperare le mie credenziali per il Portale del cliente?
{: #bicp_retcreds}

Se utilizzi l'ID IBM per l'autenticazione, quando effettui il primo ordine o quando vieni aggiunto come utente a un account, ti viene inviata un'e-mail contenente un link per iniziare con l'ID IBM. Se dimentichi o perdi il tuo nome utente o password, vai al tuo [profilo ID IBM![Icona link esterno](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} e reimposta o recupera la password utilizzando le istruzioni che seguono la procedura di accesso. Ti verrà richiesto di immettere informazioni specifiche, che potrebbero includere le risposte alle tue domande di sicurezza.

Se NON utilizzi l'ID IBM per l'autenticazione, quando effettui il primo ordine o vieni aggiunto come utente a un account del [portale del cliente ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, ricevi un'e-mail contenente il tuo nome utente e la password iniziale per iniziare nel portale del cliente. Assicurati di cambiare la password dopo aver effettuato l'accesso per la prima volta [modificando il tuo profilo utente](edit-user-profile.html).

Se dimentichi la password dopo aver effettuato l'accesso, utilizza la funzione **Password dimenticata** disponibile nella schermata di accesso del [portale del cliente ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Ti verrà richiesto di immettere informazioni specifiche, incluso un insieme di domande di sicurezza che hai specificato durante la [modifica del tuo profilo utente](edit-user-profile.html).

Se dimentichi il nome utente, contatta l'amministratore dell'account o l'utente master, che ha la possibilità di recuperare il tuo nome utente. Se sei l'amministratore o l'utente master dell'account, contatta il supporto per ricevere ulteriore assistenza.

## Che cos'è l'ID IBM e in che modo è correlato agli utenti dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_whatisibmid}

I nuovi account richiedono l'ID IBM per l'autenticazione. Gli account esistenti continuano a utilizzare il nome utente e la password SoftLayer per l'autenticazione finché non esegui lo strumento di migrazione per passare a un ID IBM. Il tuo account SoftLayer ha un utente master che ha quindi l'autorità di aggiungere più utenti all'interno dello stesso account. Per ulteriori informazioni, vedi [How SoftLayer accounts are managed in customer portal](/docs/customer-portal/cphowacctsman.html).

## Come collego un account SoftLayer esistente?
{: #bicp_linkbmxacct}

Se sei l'utente master nel tuo account SoftLayer, accedi al portale del cliente e fai clic su **Collega un account** nell'intestazione.  Per ulteriori informazioni, vedi [Collegamento degli account utente ID IBM](/docs/account/softlayerlink.html).

## Devo essere un utente {{site.data.keyword.Bluemix_notm}} esistente per collegare gli account?
{: #bicp_bmxusertolink}

No. Puoi creare un nuovo account {{site.data.keyword.Bluemix_notm}} o collegare un account di prova o con pagamento a consumo {{site.data.keyword.Bluemix_notm}} esistente.


## Come funzionerà la mia autenticazione a due fattori?
{: #bicp_2fa}

Non vi è alcun impatto sulla configurazione dell'autenticazione a due fattori a livello di account. L'autenticazione a due fattori non è per ogni ID IBM bensì per ogni account. Quando un ID IBM è associato a molti account e tu passi da un account all'altro, devi confermare la tua identità ogni volta che passi a un account diverso che richiede l'autenticazione a due fattori. Questo è vero anche se l'account precedente e il nuovo account erano entrambi configurati con lo stesso meccanismo 2FA.

Per ulteriori informazioni sull'ID IBM con l'autenticazione a due fattori, vedi [Utilizzo dell'autenticazione a due fattori negli account collegati](/docs/account/softlayerlink.html).


## Chi può collegare gli account?
{: #bicp_wholinkaccts}

Solo gli utenti master dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} possono collegare gli account SoftLayer e {{site.data.keyword.Bluemix_notm}}. È necessario inoltre associare l'e-mail di utente master al proprietario principale dell'account {{site.data.keyword.Bluemix_notm}} che viene collegato.


## Cosa devo usare per accedere a ciascun portale?
{: #bicp_logineachport}

La fatturazione dell'account è collegata e puoi spostarti facilmente tra i tuoi account SoftLayer e {{site.data.keyword.Bluemix_notm}}, ma le identità dei tuoi account rimangono separate.

* Se il tuo account non utilizza l'ID IBM per l'autenticazione, continua a usare il tuo ID SoftLayer per i prodotti e i servizi SoftLayer e il tuo ID IBM per i prodotti e i servizi {{site.data.keyword.Bluemix_notm}}.

* Se il tuo account utilizza l'ID IBM per l'autenticazione, utilizza il tuo ID IBM per accedere a entrambi i tuoi account SoftLayer e {{site.data.keyword.Bluemix_notm}}.


## Ho provato ad accedere con il mio nome utente SoftLayer, perché ricevo un errore?
{: #bicp_SLloginerror}

Dopo essere passato a un ID IBM, se accedi al portale del cliente con il tuo nome utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} visualizzerai l'errore *"Credenziali di accesso non valide"*.
Questo si verifica perché, dopo essere passato a un ID IBM, non puoi più accedere al portale del cliente con il tuo nome utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Devi invece fare clic su **Accedi con ID IBM** nella finestra di dialogo Accesso account.

## Ho provato a collegarmi con il mio ID IBM, perché ricevo un errore?
{: #bicp_IBMidloginerror}

Quando ti colleghi con il tuo ID IBM, se ricevi l'errore *"ID IBM o indirizzo e-mail non riconosciuto"*, assicurati di immettere un indirizzo e-mail completo. Assicurati inoltre di non utilizzare il tuo nome utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.


##  Ho un nuovo account SoftLayer che utilizza l'ID IBM per l'autenticazione; posso utilizzare lo stesso ID per l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} e {{site.data.keyword.Bluemix_notm}}?
{: #bicp_loginIBMidSLBlusame}

Sì, puoi utilizzare lo stesso ID IBM per accedere all'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} e a {{site.data.keyword.Bluemix_notm}}.


## Ho collegato un account {{site.data.keyword.Bluemix_notm}}, come fornisco l'accesso agli altri membri del team dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_linkgiveteamaccess}

Devi invitarli a {{site.data.keyword.Bluemix_notm}}. Nell'interfaccia utente {{site.data.keyword.Bluemix_notm}}, seleziona **Account e supporto** > **Account** > **Invita membri del team**. Dopo aver selezionato un gruppo di risorse, vedrai un'opzione per aggiungere i membri del team dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Potresti dover accedere all'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} prima di poter inviare gli inviti. {{site.data.keyword.Bluemix_notm}} richiama l'elenco degli utenti dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} e potrai quindi selezionare gli utenti da invitare all'account {{site.data.keyword.Bluemix_notm}}.


## Dov'è la mia e-mail per completare il passaggio all'Id IBM?
{: #bicp_ibmidswitchemail}

Se hai seguito la procedura guidata per passare all'ID IBM e non hai ricevuto l'e-mail, l'invio dell'e-mail con il tuo codice di registrazione può richiedere minuti o ore. Puoi tornare alla pagina **Modifica profilo utente** nel portale del cliente e fare clic su **Invia nuovamente e-mail** per riprovare.


## Avrò accesso root completo al mio account?
{: #bicp_fullrootaccaccess}

Gli utenti master e quelli con autorizzazioni di amministratore hanno accesso root completo agli account sul portale del cliente e sull'API. Gli utenti senza autorizzazioni di amministratore hanno l'accessibilità controllata da quelli con i ruoli di amministratore. Queste autorizzazioni possono essere aggiornare in qualsiasi momento [modificando il profilo utente](edit-user-profile.html) nel portale del cliente.


## Posso collegare un account di sottoscrizione {{site.data.keyword.Bluemix_notm}}?
{: #bicp_linkbmxsubacct}

Tutti gli account collegati in {{site.data.keyword.Bluemix_notm}} devono essere del tipo Pagamento a consumo. Puoi creare un nuovo account Pagamento a consumo o collegarne uno esistente. In alternativa, puoi collegare un account di prova esistente, ma verrà aggiornato a un account Pagamento a consumo.


## Come scollego il mio account {{site.data.keyword.Bluemix_notm}} dal mio account dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_unlinkacct}

Una volta che gli account sono stati collegati, non possono essere scollegati.


## Cos'è il mio profilo azienda e dove posso trovarlo?
{: #bicp_whatfindcompprof}

Il profilo azienda rappresenta le informazioni inviate al momento della creazione dell'account e include un contatto principale per l'azienda, insieme al nome, all'indirizzo e al numero di telefono della società. Queste informazioni sono utilizzate per una serie di motivi e dovrebbero essere mantenute aggiornate in ogni momento. Per visualizzare il profilo azienda per il tuo account o per richiedere modifiche, vedi [Aggiornamento del tuo profilo azienda](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch).

## Dove trovo le mie password per il dispositivo e il software?
{: #bicp_devswpw}

Le password del dispositivo e del software sono memorizzate in due posizioni all'interno del [portale del cliente ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Per recuperare le credenziali del dispositivo, inclusi il nome utente e la password root o amministratore per i {{site.data.keyword.baremetal_short}} e {{site.data.keyword.virtualmachinesshort}}, vedi [Interazione con un dispositivo nella vista dell'istantanea](/docs/vsi/vsi_interact_device_snapshot_view.html). Per visualizzare e recuperare rapidamente le credenziali del software che vengono tracciate manualmente utilizzando il portale del cliente, vedi [Gestione dell'accesso al dispositivo](/docs/vsi/vsi_device_access.html).

##Come posso mantenere sincronizzati i miei dati web?
{: #bicp_webdatasync}

Sebbene tu sia responsabile per il mantenimento della coerenza dei dati tra server reali, {{site.data.keyword.BluSoftlayer_full}} fornisce una rete privata che puoi utilizzare per sincronizzare senza incorrere in costi di utilizzo.


## Cos'è Event Management System?
{: #bicp_whatisems}

The Event Management System è un insieme di strumenti che ottimizza il modo in cui {{site.data.keyword.BluSoftlayer_full}} condivide le informazioni con gli utenti su problemi di infrastruttura non pianificati e imminenti eventi di manutenzione pianificata. Utilizza avvisi e-mail mirati basati su sottoscrizione relativi a questi incidenti per condividere il tipo di evento che si è verificato. Fornisce agli utenti sottoscritti ulteriori dettagli sull'impatto complessivo dell'evento e sullo stato corrente dell'incidente non pianificato in corso (UIP).

## Come e dove posso annullare un dispositivo?
{: #bicp_candev}

Puoi annullare un dispositivo in qualsiasi momento attraverso il [portale del cliente ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Vedi [Cancel a Device](/vsi/vsi_managing.html) per ulteriori informazioni su come completare la richiesta di annullamento.
