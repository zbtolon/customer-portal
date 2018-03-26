---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-17"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestione di un profilo utente
{: #customerportal_accuserprof}

Nel portale del cliente, un profilo utente contiene una varietà di dati sull'utente, incluse le informazioni di contatto e la chiave API. È anche il luogo in cui vengono memorizzate le password. Inoltre, se disponi dell'accesso amministrativo, puoi modificare le autorizzazioni e l'accesso al dispositivo dal profilo.
{:shortdesc}

All'interno del profilo utente, puoi gestire le informazioni di contatto e le password, visualizzare le chiavi API e aggiornare le autorizzazioni aggiuntive e l'accesso al dispositivo in base alle tue autorizzazioni. 

## Modifica di un profilo utente
{: #cp_edituserprofile}

Una volta creato un profilo utente nel portale del cliente, puoi modificarlo in qualsiasi momento. I dettagli associati al profilo utente includono informazioni personali, impostazioni di accesso, dettagli di accesso API, sottoscrizioni delle notifiche utente e domande di sicurezza. Utilizza la seguente procedura per modificare un profilo utente.

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account > Utenti** dalla barra di navigazione.
3. Fai clic sul nome utente per accedere al profilo associato a tale utente. 
4. Modifica i dettagli del **Profilo utente** secondo necessità. Per gli utenti negli account che utilizzano l'ID IBM per l'autenticazione, aggiorna l'e-mail e la password nel tuo profilo dell'ID IBM. Per ulteriori informazioni, vedi la Tabella 1.
5. Se vuoi reimpostare la tua password dopo l'accesso, fai clic su **Reimposta password** per generare un'e-mail che ti consente di modificare la password.
6. Fai clic su **Modifica utente** per inviare le modifiche.

| Campo | Definizione |
|-----|----------|
| Nome, Cognome | Nome e cognome dell'utente associato al profilo utente.|
| Indirizzo e-mail | Indirizzo e-mail preferito per ricevere notifiche dall'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} riguardanti l'account. La modifica dell'indirizzo e-mail modifica il record nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Questa modifica non influisce sul collegamento alle credenziali di autenticazione con ID IBM. Devi modificare l'indirizzo e-mail per l'ID IBM dal profilo dell'ID IBM.|
| Fuso orario | Fuso orario preferito da utilizzare durante la visualizzazione dei dati con data/ora .|
| Telefono, Telefono alternativo | Numeri di telefono di contatto preferiti che verranno utilizzati dall'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.|
| Indirizzo, Città, Paese, Stato/provincia, CAP/codice postale | Indirizzo completo di contatto che verrà utilizzato dall'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.|
{: caption="Tabella 1. Impostazioni di configurazione delle informazioni personali per la modifica di un profilo utente" caption-side="top"}

|Campo|Definizione|
|-----|----------|
| Limita accesso all'IP | Indirizzo IP a cui limitare l'accesso quando si tenta di utilizzare il portale del cliente sotto il profilo utente associato.|
| Validità password (solo per gli utenti negli account che NON utilizzano l'ID IBM per l'autenticazione) | Quantità di tempo in cui una password deve essere associata al profilo utente prima di dover selezionare una nuova password.|
| Utente principale | Account utente considerato utente principale del profilo utente. L'impostazione predefinita per l'utente principale è l'ID account primario. |
| Richiedere domande di sicurezza? | Seleziona questa casella di spunta quando devono essere richieste domande di sicurezza durante l'accesso. Se questa casella è selezionata, vengono richieste domande di sicurezza per il profilo utente.|
| Password VPN | Password da utilizzare per l'accesso VPN. Fai clic sulla casella di spunta **Utilizza password del portale per VPN** per utilizzare la password del portale del cliente per accedere alla rete dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} attraverso VPN. |
{: caption="Tabella 2. Impostazioni di configurazione delle impostazioni di accesso per la modifica di un profilo utente" caption-side="top"}

|Sezione|Campo|Definizione|
|-------|-----|----------|
| Informazioni di accesso API | IP consentiti | Indirizzi IP consentiti per l'autenticazione nell'API utilizzando la chiave API associata al profilo utente |
| Sottoscrizioni delle notifiche utente | Fatturazione | Seleziona la casella di spunta **Fatturazione** per ricevere una fattura e-mail dopo che è stata creata. |
| Domande di sicurezza | Domanda di sicurezza | Quando modifichi il tuo profilo, questa è la domanda a cui è devi rispondere per accedere se sono state attivate domande di sicurezza per il tuo profilo.
| Risposte di sicurezza | Risposta | Risposta sensibile al maiuscolo/minuscolo alla domanda di sicurezza applicabile.|
{: caption="Tabella 3. Altre impostazioni di configurazione per la modifica di un profilo utente" caption-side="top"}
Dopo aver inviato le modifiche a un profilo utente, tali modifiche vengono applicate immediatamente. Puoi modificare nuovamente il profilo utente in qualsiasi momento ripetendo i passi precedenti.  

Vedi [Passaggio all'ID IBM](/docs/account/softlayerlink.html#switching-to-ibmid) per ulteriori informazioni sulla configurazione di un account ID IBM.

## Modifica delle autorizzazioni del portale del cliente di un utente
{: #cp_editusercpperm}

Le autorizzazioni utente nel portale del cliente vengono impostate dall'amministratore dell'account quando l'utente viene aggiunto e possono essere modificate in qualsiasi momento da un utente autorizzato. Puoi modificare il tuo profilo utente e, se sei un utente amministrativo, alcuni campi dei profili utente per gli utenti che hai aggiunto. Le autorizzazioni sono suddivise in cinque schede: supporto, dispositivi, rete, servizi e account. Puoi aggiornare le autorizzazioni per un utente alla volta e devi salvare le modifiche affinché diventino attive. 

Utilizza la seguente procedura per modificare le autorizzazioni del portale del cliente di un utente.

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account > Utenti** dalla barra di navigazione.
3. Fare clic sul nome dell'utente per accedere al profilo utente.
4. Fai clic sull'icona **Autorizzazioni** per accedere alla finestra Autorizzazioni.

  Potresti ricevere un messaggio che indica che le modifiche non sono state salvate nel profilo utente. Se al profilo non è stata apportata alcuna modifica, fai clic per ignorare le modifiche e accedere alla finestra Autorizzazioni.
  {: tip}

5. Seleziona le autorizzazioni:
  * Per impostare autorizzazioni rapide, seleziona la serie di autorizzazioni dall'elenco **Autorizzazioni rapide**. Dopo aver selezionato una serie di autorizzazioni, ogni autorizzazione associata alla serie viene visualizzata in testo arancione con una freccia arancione che punta alla casella di spunta. Fai quindi clic su **Imposta autorizzazioni** per ciascuna scheda.
  * Per impostare singole autorizzazioni, seleziona o deseleziona ciascuna casella di spunta sulle schede per aggiornare le autorizzazioni dell'utente. Fai clic su **Seleziona tutte le autorizzazioni** o **Deseleziona tutte le autorizzazioni** su ciascuna scheda per selezionare o deselezionare tutte le autorizzazioni contemporaneamente.
6. Fai clic su **Modifica autorizzazioni del portale** per inviare le modifiche e aggiornare le autorizzazioni dell'utente.
7. Per reimpostare le autorizzazioni dell'utente alle impostazioni originali invece di salvarle, fai clic su **Reimposta autorizzazioni**. Fai clic su **Annulla** per annullare le modifiche e tornare alla finestra Utenti.

Le autorizzazioni utente vengono aggiornate immediatamente dopo l'invio delle modifiche. Se sono state concesse le autorizzazioni, l'utente può visualizzare o interagire con le funzioni selezionate. Se le autorizzazioni sono state rimosse, l'utente non può più visualizzare o interagire con le funzioni selezionate. Le autorizzazioni possono essere aggiornate di nuovo in qualsiasi momento ripetendo i passi precedenti. 

## Aggiunta dell'autenticazione esterna per un utente
{: #cp_addextauthuser}

Dal portale del cliente, puoi attivare l'autenticazione esterna a due fattori per aggiungere ulteriore protezione durante l'accesso al portale. Questo ulteriore livello di sicurezza protegge l'account da accessi non verificati, garantendo la protezione di dispositivi, dati e informazioni sull'account. Questa autenticazione esterna è disponibile nelle seguenti forme:

* **Symantec Identify Protection** è lo strumento di autenticazione esterna più comune che fornisce un codice di sicurezza dinamico utilizzato in aggiunta al nome utente e alla password quando si accede al portale del cliente. 
* L'autenticazione **PhoneFactor** fornisce l'autenticazione utente fuori banda da un telefono, un SMS o un'applicazione mobile. PhoneFactor richiede un numero di telefono valido a cui devi avere accesso ogni volta che tenti di eseguire l'autenticazione.

Puoi aggiungere entrambi i metodi di autenticazione esterna, per ogni utente, con una [piccola quota mensile ![Icona link esterno](../icons/launch-glyph.svg)](http://www.softlayer.com/services/security/){:new_window}. Utilizza la seguente procedura per aggiungere l'autenticazione esterna per un utente del portale del cliente.

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account > Utenti** dalla barra di navigazione.
3. Seleziona **Aggiungi autenticazione esterna** dall'elenco **Azioni** per l'utente.
4. Seleziona il tipo di autenticazione esterna da ordinare:
  * **Symantec Identity Protection** -- Immetti l'ID credenziale dell'utente nel campo **ID credenziale**.
  * **PhoneFactor** -- Scegli un [metodo di autenticazione](#cp_phonefacauthmeths).
5. Fai clic su **Continua**.
6. Completa i prompt nella finestra per **Codice promozionale** e **Riconoscimento MSA**.
7. Fai clic su **Ordina autenticazione esterna** per completare l'ordine.

Dopo aver aggiunto l'autenticazione esterna per un utente, i passi successivi dipendono dal tipo di autenticazione.
* Se è abilitato Symantec Identity Protection, devi aggiungere il codice di sicurezza associato all'ID credenziale dell'utente immesso nel sistema nel momento in cui Symantec Identity Protection è stato aggiunto all'account.
* Se è abilitato PhoneFactor, l'utente deve [attivare PhoneFactor](#cp_actphonefacauth) per utilizzare questo tipo di autenticazione a due fattori con l'account.

### Attivazione dell'autenticazione PhoneFactor
{: #cp_actphonefacauth}

Dopo aver aggiunto PhoneFactor, devi attivare manualmente l'autenticazione esterna con PhoneFactor attraverso il portale del cliente. Poiché PhoneFactor utilizza il contatto manuale, è importante assicurarsi che tutti i numeri di telefono associati all'account siano sempre aggiornati. Il mancato aggiornamento delle informazioni di contatto potrebbe comportare l'impossibilità di accedere al portale del cliente e alla VPN quando PhoneFactor è attivo. Una volta che PhoneFactor è stato aggiunto correttamente, riceverai un'e-mail di conferma. Dopo aver ricevuto l'e-mail, utilizza la seguente procedura per attivare l'autenticazione PhoneFactor.

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account > Utenti** dalla barra di navigazione.
3. Fai clic sul nome utente per accedere al profilo associato a tale utente. 
4. Scorri fino alla sezione **Impostazioni PhoneFactor**.

  Se la sezione Impostazioni PhoneFactor non è disponibile, verifica innanzitutto di aver ricevuto l'e-mail di provisioning di PhoneFactor che indica che PhoneFactor è stato fornito. Se il provisioning di PhoneFactor è stato eseguito ma la sezione non è disponibile, crea un ticket di supporto. Se il provisiong di PhoneFactor non è stato ancora eseguito, attendi l'e-mail e prova di nuovo. Se PhoneFactor non è stato ancora aggiunto, vedi [Aggiunta dell'autenticazione esterna per un utente](/docs/customer-portal/cpmanuserprof.html#cp_addextauthuser).
  {: tip}

5. Seleziona **Attivo** dall'elenco **Stato**.
6. Modifica il **Numero di telefono principale** per l'autenticazione.
  1. Fai clic sul link **Modifica**.
  2. Immetti il **Codice paese**, **Numero di telefono** e l'**Estensione**, se applicabile, nei campi associati.
  3. Fai clic su **Autentica e salva numero** per completare l'autenticazione.

    Quando aggiungi un numero di telefono per l'autenticazione, devi essere al telefono. Dopo aver fatto clic su **Autentica**, viene chiamato il numero e ti viene richiesto di completare un passaggio per autenticare il numero. I numeri di telefono non possono essere autenticati senza il completamento di questi passaggi.
    {: tip}

  4. Per aggiungere un **Numero di telefono secondario**, ripeti questi passi.
7. Seleziona il **Metodo di contatto** dall'elenco **Metodo**.
8. Seleziona un **Tipo di PIN** dall'elenco **Tipo di PIN**.
9. Se selezioni **Monouso** > **Valore PIN**, immetti il PIN nel campo **Valore PIN**.
10. Fai clic su **Aggiorna** per aggiornare le modifiche e attivare l'autenticazione PhoneFactor.

Dopo l'attivazione di PhoneFactor, l'autenticazione tramite PhoneFactor è richiesta dal portale del cliente o VPN. Dopo l'autenticazione con le credenziali dell'utente, un messaggio ti indica che si sta tentando l'autenticazione PhoneFactor. È necessario che tu, o l'utente che stai aggiungendo, sia vicino al telefono elencato con PhoneFactor per completare l'autenticazione. PhoneFactor tenta l'autenticazione cinque volte. Dopo cinque tentativi di autenticazione non riusciti, verrai bloccato per circa un'ora. Tu o un utente con accesso amministrativo all'account potete modificare le impostazioni di autenticazione PhoneFactor in qualsiasi momento.  Tu o un amministratore dell'account potete disattivare PhoneFactor in qualsiasi momento.

#### Metodi di autenticazione PhoneFactor
{: #cp_phonefacauthmeths}

Se configuri PhoneFactor come tipo di autenticazione, puoi scegliere una delle seguenti opzioni come metodo di autenticazione:
<dl>
<dt>Telefonata e standard (senza pin)</dt>
<dd>Con questa opzione abilitata, quando accedi al portale, ricevi una chiamata al numero principale abilitato. Quando rispondi alla chiamata, ti viene richiesto di premere il tasto # per completare l'autenticazione.</dd>
<dt>Telefonata con pin</dt>
<dd>Con questa opzione selezionata, immetti un valore pin nel portale del cliente. Il pin deve essere compreso tra 4 e 8 numeri. Quando tenti di accedere al portale, riceve una chiamata al numero principale elencato nel portale. Quando rispondi, ti viene indicato di immettere il tuo numero pin seguito dal simbolo # per completare l'autenticazione.</dd>
<dt>Testo SMS e pin monouso</dt>
<dd>Con questa opzione selezionata, ricevi un messaggio di testo con un pin che utilizzi per rispondere al messaggio. Quando immetti il pin fornito, il processo di autenticazione viene completato e puoi accedere al portale.</dd>
<dt>Testo SMS con monouso e valore pin</dt>
<dd>Con questa opzione selezionata, crea un valore di pin da 4 a 8 numeri. Riceverai quindi un messaggio di testo e risponderai con il codice fornito e il tuo numero pin senza spazi.</dd>
<dt>Applicazione PhoneFactor e standard (senza pin)</dt>
<dd>Apri l'applicazione PhoneFactor (Azure Authenticator) sul tuo dispositivo e fai clic su  <strong>Autentica</strong>. Verrà visualizzato che sei stato autenticato correttamente utilizzando PhoneFactor e potrai accedere al portale.</dd>
<dt>Applicazione PhoneFactor con pin</dt>
<dd>Con questa opzione, imposta un pin, compreso tra 4 e 8 numeri, nel portale. Viene quindi visualizzata l'applicazione PhoneFactor (Azure Authenticator) sul tuo dispositivo. Successivamente, immetti il tuo pin creato nel portale e fai clic su <strong>Autentica</strong> per accedere al portale.</dd>
</dl>

## Modifica dello stato di un utente
{: #cp_changeuserstat}

Il tuo stato nel portale del clienti determina la tua accessibilità al tale portale. Le categorie di stato che puoi aggiornare sull'account includono Attivo, Disabilitato e Solo VPN. Il tuo stato potrebbe essere modificato per vari motivi e può essere aggiornato in qualsiasi momento. Le categorie di stato del cliente includono quelle che gli utenti possono aggiornare e quelle che vengono aggiornate automaticamente. Queste sono:
<dl>
<dt>Attivo</dt>
<dd>L'utente ha accesso completo al portale del cliente e alla VPN in base alle autorizzazioni impostate dall'amministratore dell'account. Questo stato può essere selezionato manualmente o modificato in qualsiasi momento.</dd>
<dt>Disabilitato</dt>
<dd>L'utente non ha accesso ad alcuna autorizzazione o sottoscrizione sull'account, inclusi il portale del cliente e la VPN. Se la categoria di stato viene impostata su Disabilitato da un altro utente sull'account, questo stato può essere selezionato manualmente o modificato in qualsiasi momento.</dd>
<dt>Solo VPN</dt>
<dd>L'utente ha accesso completo alla connettività VPN, in base alla propria serie di autorizzazioni, ma non può accedere al portale clienti. Questo stato può essere selezionato manualmente o modificato in qualsiasi momento.</dd>
<dt>Inattivo</dt>
<dd>L'utente non ha effettuato l'accesso al portale del cliente o alla VPN negli ultimi 60 giorni. Questo è uno stato generato dal sistema.</dd>
<dt>cancel_pending</dt>
<dd>Un amministratore dell'account ha cancellato questo utente e la cancellazione è attualmente in fase di elaborazione. Questo è uno stato generato dal sistema.</dd>
</dl>

Utilizza la seguente procedura per modificare lo stato dell'utente nel portale del cliente.

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Utenti** dalla barra di navigazione.
3. Seleziona **Modifica stato utente** dall'elenco **Azioni**.
4. Dall'elenco **Stato**, seleziona  lo stato appropriato in base alle definizioni nell'elenco precedente.
5. Fai clic su **Salva**.

Dopo aver aggiornato lo stato di un utente, le modifiche all'accessibilità del portale clienti si allineano con il nuovo stato.

## Modifica dell'accesso VPN di un utente
{: #cp_edituservpnaccess}

Quando un [nuovo utente viene aggiunto](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct) a un account del portale del cliente, l'accesso VPN viene selezionato tra una varietà di metodi di connessione, tra cui SSL, PPTP o una combinazione dei due. Con l'accesso VPN, è possibile accedere alla rete privata nella sua interezza o l'accesso alla rete può essere limitato a una o più sottoreti specifiche. Puoi gestire e aggiornare l'accesso VPN in qualsiasi momento dalla finestra Utenti. Utilizza la seguente procedura per modificare l'accesso VPN di un utente.

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Accesso VPN** dalla barra di navigazione.
3. Dalla colonna **Accesso VPN** relativa all'utente, fai clic sul link del tipo di accesso VPN corrente per visualizzare la finestra Accesso VPN.
4. Dall'elenco **Tipo di VPN**, seleziona un metodo VPN (SSL, PPTP, SSL & PPTP o nessuno) da assegnare all'utente.
5. Indica come deve essere gestito l'**Accesso alla sottorete**:
  * Seleziona **Automatico** per gestire automaticamente l'accesso alla sottorete
  * Seleziona **Manuale** per gestire manualmente l'accesso alla sottorete e quindi seleziona la casella di spunta **Concedi accesso** per ogni sottorete a cui l'utente dovrà avere accesso. Assicurati di deselezionare le caselle di spunta a cui l'utente non deve avere accesso.
6. Fai clic su **Salva**.

Dopo aver aggiornato l'accesso VPN di un utente, le relative autorizzazioni vengono aggiornate di conseguenza e la colonna Accesso VPN visualizza il metodo di accesso VPN aggiornato, laddove applicabile. 

### Attivazione o disattivazione dell'accesso VPN
{: #cp_pptpvpn}

Puoi attivare la VPN PPTP per creare un tunnel sicuro sulla rete privata dell'infrastruttura {{site.data.keyword.BluSoftlayer_full}} utilizzando il software client specializzato in esecuzione sul tuo desktop o dispositivo dedicato. Puoi usare PPTP se hai bisogno di connettere il tuo intero ufficio o se non puoi utilizzare la soluzione VPN SSL.

Ti viene assegnata una connessione PPTP con connessioni aggiuntive disponibili. Puoi richiedere il supporto per abilitare l'accesso PPTP illimitato, che è disponibile senza costi aggiuntivi. Utilizza la seguente procedura per attivare o disattivare l'accesso VPN PPTP:

1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Accesso VPN** dalla barra dei menu.
3. Dalla colonna **Accesso VPN** relativa all'utente, fai clic sul link del tipo di accesso VPN corrente per visualizzare la finestra Accesso VPN.
4. Dall'elenco **Tipo di VPN**, seleziona un metodo VPN (SSL, PPTP, SSL & PPTP o nessuno) da assegnare all'utente.

## Impostazione dell'opzione Supportato UE
{: #cp_seteusupported}

Puoi indicare che desideri ricevere assistenza esclusivamente da un team di supporto che si trova fisicamente nell'Unione Europea (UE). Puoi selezionare questa opzione quando configuri il tuo account o quando aggiorni il tuo account esistente. Per impostare l'opzione **Supportato UE**, utilizza la seguente procedura:
1. Accedi al portale del cliente utilizzando le tue credenziali univoche.
2. Fai clic su **Account** > **Gestisci** > **Profilo azienda** dalla barra dei menu.
3. Seleziona la casella di spunta **Supportato UE**.
4. Fai clic su **Richiedi aggiornamento profilo**.

Se l'opzione **Supportato UE** non è disponibile, è possibile che ci siano utenti nel tuo account con l'accesso VPN PPTP abilitato. Disabilita l'accesso VPN PPTP per tutti gli utenti nel tuo account per abilitare l'opzione **Supportato UE**. Per ulteriori informazioni, vedi [Attivazione o disattivazione dell'accesso VPN PPTP](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn).

Per ulteriori informazioni sull'implementazione dell'opzione **Supportato UE** quando apri un ticket di supporto, vedi [Richiesta di supporto per le risorse nell'Unione Europea](/docs/get-support/howtogetsupport.html#eusupported).
