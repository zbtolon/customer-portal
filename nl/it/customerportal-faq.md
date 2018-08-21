---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-16"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# FAQ
{: #bicpfaq}

## Come richiamo le mie credenziali per il portale clienti?
{: #bicp_retcreds}

Se utilizzi l'ID IBM per l'autenticazione, quando effettui il primo ordine o quando vieni aggiunto come utente a un account, ricevi un'e-mail contenente un link per iniziare con l'ID IBM. Se dimentichi o perdi il tuo nome utente o la tua password, vai al tuo [profilo ID IBM![Icona link esterno](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} e reimposta o recupera la password utilizzando le istruzioni che seguono la procedura di accesso. Ti viene richiesto di immettere informazioni specifiche, che potrebbero includere le risposte alle tue domande di sicurezza.

Se non utilizzi l'ID IBM per l'autenticazione, quando effettui il primo ordine o vieni aggiunto come utente a un account del [portale clienti ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, ricevi un'e-mail contenente il tuo nome utente e la password iniziale per iniziare nel portale clienti. Assicurati di cambiare la tua password dopo aver effettuato l'accesso per la prima volta modificando il tuo profilo utente. 

Se dimentichi la tua password dopo aver effettuato l'accesso, utilizza la funzione **Password dimenticata** disponibile nella schermata di accesso del portale clienti. Ti viene richiesto di immettere delle informazioni specifiche, comprese una serie di domande di sicurezza da te specificate quando hai configurato il tuo profilo utente.

Se dimentichi il nome utente, contatta l'amministratore dell'account o l'utente master, che ha la possibilità di recuperare il tuo nome utente. Se sei l'amministratore o l'utente master dell'account, contatta il supporto per ricevere ulteriore assistenza.

## Cos'è l'ID IBM?
{: #bicp_whatisibmid}

I nuovi account richiedono l'ID IBM per l'autenticazione. Gli account esistenti continuano a utilizzare il nome utente e la password SoftLayer per l'autenticazione finché non esegui lo strumento di migrazione per passare a un ID IBM. Il tuo account SoftLayer ha un utente master che ha quindi l'autorità di aggiungere più utenti all'interno dello stesso account. Per ulteriori informazioni, vedi [How SoftLayer accounts are managed in customer portal](/docs/customer-portal/cphowacctsman.html).

## Come collego un account SoftLayer esistente?
{: #bicp_linkbmxacct}

Se sei l'utente master nel tuo account SoftLayer, esegui l'accesso al portale clienti e fai clic su **Collega un account** nell'intestazione.  Per ulteriori informazioni, vedi [Collegamento degli account utente ID IBM](/docs/account/softlayerlink.html).

## Devo essere un utente {{site.data.keyword.Bluemix_notm}} esistente per collegare gli account?
{: #bicp_bmxusertolink}

No. Puoi creare un nuovo account {{site.data.keyword.Bluemix_notm}} o collegare un account Lite o Pagamento a consumo {{site.data.keyword.Bluemix_notm}} esistente.

## Come funziona l'autenticazione a due fattori?
{: #bicp_2fa}

Non vi è alcun impatto sulla configurazione dell'autenticazione a due fattori (2FA) a livello di account. 2FA non è per ogni ID IBM bensì per ogni account. Quando un ID IBM è associato a molti account e tu passi da un account all'altro, devi confermare la tua identità ogni volta che passi a un account diverso che richiede la 2FA. Questo è vero anche se l'account precedente e il nuovo account sono entrambi configurati con lo stesso meccanismo 2FA.

Per ulteriori informazioni sull'ID IBM con la 2FA, vedi [Utilizzo dell'autenticazione a due fattori negli account collegati](/docs/account/softlayerlink.html).

## Chi può collegare gli account?
{: #bicp_wholinkaccts}

Solo gli utenti master dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} possono collegare gli account SoftLayer e {{site.data.keyword.Bluemix_notm}}. È necessario inoltre associare l'e-mail di utente master al proprietario principale dell'account {{site.data.keyword.Bluemix_notm}} che viene collegato.

## Cosa utilizzerò per eseguire l'accesso a ciascuna console?
{: #bicp_logineachport}

La fatturazione dell'account è collegata e puoi spostarti facilmente tra i tuoi account SoftLayer e {{site.data.keyword.Bluemix_notm}}, ma le identità dei tuoi account rimangono separate.

* Se il tuo account non utilizza l'ID IBM per l'autenticazione, continua a usare il tuo ID SoftLayer per i prodotti e i servizi SoftLayer e il tuo ID IBM per i prodotti e i servizi {{site.data.keyword.Bluemix_notm}}.

* Se il tuo account utilizza l'ID IBM per l'autenticazione, utilizza il tuo ID IBM per accedere a entrambi i tuoi account SoftLayer e {{site.data.keyword.Bluemix_notm}}.

## Perché ottengo un errore quando provo ad eseguire l'accesso con il mio nome utente SoftLayer?
{: #bicp_SLloginerror}

Una volta che passi a un ID IBM, se esegui l'accesso al portale clienti con il tuo nome utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}, viene visualizzato l'errore "Invalid login credentials provided". Una volta che passi a un ID IBM, non puoi più eseguire l'accesso al portale clienti con il tuo nome utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Devi invece fare clic su **Accedi con ID IBM** nella finestra di dialogo Accesso account.

## Perché ottengo un errore quando provo ad eseguire l'accesso con il mio ID IBM?
{: #bicp_IBMidloginerror}

Quando esegui l'accesso con il tuo ID IBM, viene visualizzato l'errore "We didn't recognize this IBMid or email". Assicurati di immettere un indirizzo email completo. Assicurati inoltre di non utilizzare il tuo nome utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.

## I membri del team dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} possono accedere al mio account collegato?
{: #bicp_linkgiveteamaccess}

Devi invitarli a {{site.data.keyword.Bluemix_notm}}. Nella console {{site.data.keyword.Bluemix_notm}}, fai clic su **Gestisci** > **Account** > **Utenti**. Dopo che hai selezionato un gruppo di risorse, puoi aggiungere i membri del team dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Potresti dover accedere al portale clienti prima di poter inviare gli inviti. {{site.data.keyword.Bluemix_notm}} richiama l'elenco degli utenti dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} e potrai quindi selezionare gli utenti da invitare all'account {{site.data.keyword.Bluemix_notm}}.

## Dov'è la mia e-mail per completare il passaggio all'Id IBM?
{: #bicp_ibmidswitchemail}

Se hai seguito la procedura guidata per passare all'ID IBM e non hai ricevuto l'e-mail, l'invio dell'e-mail con il tuo codice di registrazione può richiedere minuti o ore. Puoi tornare alla pagina **Modifica profilo utente** nel portale clienti e fare clic su **Invia nuovamente e-mail** per riprovare.

## Avrò accesso root completo al mio account?
{: #bicp_fullrootaccaccess}

Gli utenti master e quelli con autorizzazioni di amministratore hanno accesso root completo agli account sul portale clienti e sull'API. Gli utenti senza autorizzazioni di amministratore hanno l'accessibilità controllata da quelli con i ruoli di amministratore. Queste autorizzazioni possono essere aggiornate dagli amministratori dal portale clienti [modificando un profilo utente](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Senza le autorizzazioni di amministratore, puoi modificare il tuo profilo utente nel portale clienti facendo clic sul tuo nome utente nel pannello superiore.

## Posso collegare un account Sottoscrizione {{site.data.keyword.Bluemix_notm}}?
{: #bicp_linkbmxsubacct}

Tutti gli account collegati in {{site.data.keyword.Bluemix_notm}} devono essere account Lite o Pagamento a consumo. 

## Come annullo il collegamento del mio account?
{: #bicp_unlinkacct}

Una volta che gli account sono stati collegati, non possono essere scollegati.


## Cos'è il mio profilo azienda e dove posso trovarlo?
{: #bicp_whatfindcompprof}

Il profilo azienda rappresenta le informazioni inviate al momento della creazione dell'account e include un contatto principale per l'azienda, insieme al nome, all'indirizzo e al numero di telefono dell'azienda. Queste informazioni sono utilizzate per una serie di motivi e dovrebbero essere mantenute aggiornate in ogni momento. Per visualizzare il profilo azienda per il tuo account o per richiedere modifiche, vedi [Aggiornamento del tuo profilo azienda](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch).

## Dove trovo le mie password per il dispositivo e il software?
{: #bicp_devswpw}

Le password del dispositivo e del software vengono archiviate in due ubicazioni all'interno del portale clienti. Per recuperare le credenziali del dispositivo, inclusi il nome utente e la password root o amministratore per i {{site.data.keyword.baremetal_short}} e {{site.data.keyword.virtualmachinesshort}}, vedi [Interazione con un dispositivo nella vista dell'istantanea](/docs/vsi/vsi_interact_device_snapshot_view.html). Per visualizzare e richiamare rapidamente le credenziali del software che vengono tracciate manualmente utilizzando il portale clienti, vedi [Gestione dell'accesso al dispositivo](/docs/vsi/vsi_device_access.html).

## Come posso mantenere sincronizzati i miei dati web?
{: #bicp_webdatasync}

Sebbene tu sia responsabile per il mantenimento della congruenza dei dati tra server reali, {{site.data.keyword.BluSoftlayer_full}} fornisce una rete privata che puoi utilizzare per eseguire la sincronizzazione senza incorrere in costi di utilizzo.

## Cos'è Event Management System?
{: #bicp_whatisems}

Event Management System è un insieme di strumenti che ottimizza il modo in cui {{site.data.keyword.BluSoftlayer_full}} condivide le informazioni con gli utenti su problemi di infrastruttura non pianificati e imminenti eventi di manutenzione pianificata. Utilizza avvisi e-mail mirati basati su sottoscrizione relativi a questi incidenti per condividere il tipo di evento che si è verificato. Fornisce agli utenti sottoscritti ulteriori dettagli sull'impatto complessivo dell'evento e sullo stato corrente dell'incidente non pianificato in corso (UIP).

## Posso annullare un dispositivo?
{: #bicp_candev}

Puoi annullare un dispositivo in qualsiasi momento tramite il portale clienti. Vedi [Annulla un dispositivo](/docs/vsi/vsi_managing.html) per ulteriori informazioni su come completare la richiesta di annullamento.
