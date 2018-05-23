---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Aggiunta di utenti a un account SoftLayer
{: #customerportal_addusertocpacct}

Uno o più utenti possono interagire con i prodotti e i servizi associati a un account. Se sei l'utente master, puoi aggiungere utenti in qualsiasi momento.
{:shortdesc}

Se gestisci gli utenti dell'infrastruttura {{site.data.keyword.BluSoftlayer_full}}, quali account SoftLayer puoi gestire dipende dall'accesso che è stato assegnato al tuo account utente e da come è configurato il tuo account. Se sei l'utente master o hai un accesso amministrativo come proprietario dell'account, puoi gestire altri utenti del portale clienti. Se il tuo account non è configurato come utente master, puoi gestire il tuo profilo utente.

A seconda del tuo accesso, puoi gestire il tuo account SoftLayer o gli account di altri utenti dalla finestra Utenti. La finestra Utenti nel [portale clienti ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} visualizza gli utenti associati a un account. Le interazioni disponibili nella finestra Utenti variano in base alla tua serie univoca di autorizzazioni account.
  * Se sei l'utente master dell'account, puoi visualizzare tutti gli utenti associati all'account.

  Se devi condividere le credenziali di accesso master per il tuo account, condividi le credenziali con attenzione. Il tuo accesso master controlla ogni aspetto del tuo account e deve essere protetto. Per consentire ad altri utenti di utilizzare il portale clienti, puoi configurare utenti individuali o basati su autorizzazioni. Ciò ti consente di avere il massimo controllo su chi è in grado di interagire con determinati aspetti del tuo account.
{:tip}

  * Se disponi dell'accesso amministrativo, puoi vedere tutti gli utenti che hai creato e, se hai concesso a tali utenti l'autorizzazione per amministrare altri utenti, puoi anche vedere tutti gli utenti che essi hanno creato. Puoi anche intraprendere azioni su qualsiasi utente associato all'account, incluso la modifica dell'accesso al portale clienti, la modifica dello stato dell'utente e la rimozione di utenti.
  * Se non sei l'utente master dell'account e non disponi dell'accesso amministrativo, viene visualizzato solo il tuo profilo.  Puoi interagire con il tuo proprio account, ad esempio visualizzare la chiave API, modificare l'accesso VPN e aggiungere l'autenticazione esterna.

Per gestire gli utenti dalla console {{site.data.keyword.Bluemix_notm}}, vedi la sezione [Configurazione account](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) e [Gestione di identità e accesso](/docs/iam/quickstart.html#getstarted). Per ulteriori informazioni sulla console {{site.data.keyword.Bluemix_notm}}, vedi [Come funziona la console {{site.data.keyword.Bluemix_notm}}](/docs/overview/ui.html#ui).

Persone diverse all'interno di un'organizzazione hanno ruoli e responsabilità differenti e le serie di autorizzazioni utente non sono valide per tutti. Pertanto, puoi aggiungere utenti al portale clienti con dei ruoli per garantire che ogni persona o gruppo abbia accesso solo a ciò che deve. Se vengono apportate modifiche per errore o che non sono autorizzate, puoi risalire all'utente o al gruppo per garantire di poter fornire la formazione adeguata o aggiornare le autorizzazioni utente. Ciò minimizza i rischi in vari modi e consente agli utenti di concentrarsi sul ruolo specificato all'interno del portale clienti.

Utilizza la seguente procedura per aggiungere un utente a un account.

1. Accedi al portale clienti utilizzando le tue credenziali univoche.
2. Seleziona **Account > Utenti** dalla barra di navigazione.
3. Fai clic su **Aggiungi utente**.
4. Completa i campi obbligatori nella sezione **Informazioni personali**, compreso lo stato, un nome utente e l'indirizzo e-mail per le comunicazioni e le notifiche del portale clienti, inclusa la notifica iniziale per impostare una password per l'account.

  Facoltativamente, anziché inserire un indirizzo per l'utente, puoi fare clic sulla casella di spunta **Utilizza informazioni azienda predefinite** per compilare l'indirizzo dell'azienda.
  {: tip}

5. Completa i campi obbligatori nella sezione **Impostazioni di accesso**, indicando anche se le impostazioni possono essere modificate dall'utente, se l'indirizzo IP è limitato e se all'utente è richiesto o meno di configurare e utilizzare le domande di sicurezza. Inoltre, per tutti gli utenti che non utilizzano l'ID IBM, puoi impostare il periodo di tempo prima che la password scada.
**Note:**
* Se utilizzi l'ID IBM per l'autenticazione, aggiorna le password nei tuoi [profili ID IBM ![Icona link esterno](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} seguendo le istruzioni in **Accedi**.
* Fai clic sulla casella di spunta **Utilizza password del portale per VPN** per sincronizzare le password del portale clienti e della VPN.
6. Fai clic su **Aggiungi utente**.

Dopo aver creato un account per un utente, l'utente riceve una notifica via e-mail per completare la configurazione del proprio account impostando una password e, facoltativamente, le domande di sicurezza se hai indicato che sono richieste.

Il modo in cui gli utenti senza l'accesso amministrativo di un utente master accedono al portale clienti dipende dall'utente master che ha fornito l'accesso all'utente nei propri account SoftLayer:
  * Se l'utente master ha un ID IBM per l'autenticazione, ogni utente creato dall'utente master ha un ID IBM.
  * Se l'utente master ha un ID dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} per l'autenticazione, ogni utente creato dall'utente master ha un nome utente per l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. L'utente master e ciascun utente creato dall'utente master devono eseguire lo strumento di migrazione per passare a un ID IBM.
  * Se nessuno di questi casi è applicabile, ad esempio nel caso di business partner IBM, contatta il supporto per determinare quale ID utente utilizzare.

## Impostazioni delle autorizzazioni utente per l'account
{: #cp_setuserpermsacct}

Utilizza la seguente procedura per impostare le autorizzazioni per l'utente che hai aggiunto.

1. Fai clic sull'icona **Autorizzazioni**, indicata da una figura utente con un lucchetto.
2. Aggiorna le **Autorizzazioni utente** in tutte le schede per il nuovo utente.
> **Nota:** seleziona un'opzione dall'elenco **Autorizzazioni rapide** per visualizzare le serie di autorizzazioni consigliate per tre tipi di utenti. Fai clic su **Imposta autorizzazioni** per selezionare la serie di autorizzazioni consigliata oppure personalizza l'accessibilità dell'utente selezionando le singole opzioni in ogni scheda disponibile.
3. Fai clic su **Aggiungi autorizzazioni portale** per aggiungere le autorizzazioni o su **Reimposta autorizzazioni** per reimpostare le autorizzazioni per l'utente.
4. Fai clic sull'icona **Accesso dispositivo**, indicata da tre server.
5. Fai clic sulla casella di spunta del dispositivo per ciascun dispositivo a cui desideri che l'utente possa accedere.
6. Fai clic su **Aggiorna accesso dispositivo** dopo aver selezionato i dispositivi.

Riceverai un'e-mail con link e informazioni che ti guideranno attraverso la configurazione di un ID IBM per l'autenticazione in questo account. I passi possono includere la creazione di un nuovo ID IBM se l'account utilizza l'ID IBM per l'autenticazione. L'invito scade dopo 7 giorni, ma puoi contattare l'amministratore per un nuovo invio dell'invito.

Per tutti gli altri casi di autenticazione, dopo aver aggiunto il nuovo utente, l'utente può accedere al portale clienti in qualsiasi momento per lavorare con vari prodotti e servizi associati all'account. Puoi disattivare l'utente in qualsiasi momento.
