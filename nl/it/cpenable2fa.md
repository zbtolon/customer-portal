---

copyright:

  years: 2018

lastupdated: "2018-05-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Configurazione dell'autenticazione a due fattori
{: #customerportal_2fa}

Nel portale clienti, è possibile attivare l'autenticazione a due fattori (2FA, two-factor authentication) esterna per aggiungere ulteriore protezione quando si esegue l'accesso al portale. Questo ulteriore livello di sicurezza protegge l'account da accessi non verificati, garantendo la protezione di dispositivi, dati e informazioni sull'account.
{:shortdesc}

Se abiliti la 2FA nel portale clienti per il tuo account SoftLayer esistente, devi immettere il tuo codice di sicurezza quando esegui l'accesso alla console {{site.data.keyword.Bluemix_notm}}. Tuttavia, la 2FA si applica solo alle risorse dell'infrastruttura nel tuo account {{site.data.keyword.Bluemix_notm}}. Pertanto, potresti essere in grado di eseguire diverse azioni per le risorse nel tuo account {{site.data.keyword.Bluemix_notm}} senza completare la 2FA.

La 2FA per il tuo account SoftLayer non è per ogni ID IBM ma ancora per ogni account. Quando un ID IBM è associato a più account e tu passi da un account all'altro, devi confermare la tua identità ogni volta che passi a un account diverso. Questo è vero anche se l'account precedente e il nuovo account sono entrambi configurati con lo stesso meccanismo 2FA.

## Abilitazione della 2FA

L'autenticazione 2FA è disponibile in due formati. Entrambi i metodi di autenticazione esterna possono essere aggiunti per ogni utente per un piccolo addebito mensile:

* Symantec Identify Protection è il nostro strumento di autenticazione esterna più comune che fornisce un codice di sicurezza dinamico utilizzato in aggiunta al nome utente e alla password quando si accede al Portale clienti.
* L'autenticazione PhoneFactor fornisce l'autenticazione utente fuori banda tramite telefono, SMS o applicazione mobile.

 Se hai un account collegato, puoi avvalerti dell'impostazione di autenticazione multifattore (MFA, multi-factor authentication) [abilitando l'autenticazione multifattore](/docs/iam/mfa.html) per tutto il tuo account {{site.data.keyword.Bluemix_notm}}.
 {: tip}

Per configurare la 2FA, completa la seguente procedura:

1. Accedi alla schermata **Utenti** nel portale clienti. 
2. Seleziona **Aggiungi autenticazione esterna** dal menu **Azioni** per l'utente desiderato.
3. In base al tipo di autenticazione esterna ordinato, completa la seguente procedura:
    * Se scegli Symantec Identity Protection, seleziona **Symantec Identity Protection** e immetti quindi l'ID credenziale dell'utente.
    * Se scegli PhoneFactor, seleziona **PhoneFactor**.
4. Fai clic su **Continua**.
5. Completa i prompt nella schermata per Codice promozionale e Riconoscimento MSA.
6. Fai clic su **Ordina autenticazione esterna** per completare l'ordine. Fai clic su **Annulla** per annullare l'azione.

## Passi successivi
{: #2fanextsteps}

Dopo aver aggiunto l'autenticazione esterna per un utente, i passi successivi dipendono dal tipo di autenticazione.
* Se è abilitato Symantec Identity Protection, devi aggiungere il codice di sicurezza associato all'ID credenziale dell'utente immesso nel sistema nel momento in cui Symantec Identity Protection è stato aggiunto all'account.
* Se è abilitato PhoneFactor, l'utente deve attivare PhoneFactor per utilizzare questo tipo di autenticazione a due fattori con l'account.

### Attivazione dell'autenticazione PhoneFactor
{: #cp_actphonefacauth}

Dopo aver aggiunto PhoneFactor, devi attivare manualmente l'autenticazione esterna con PhoneFactor attraverso il portale clienti. Poiché PhoneFactor utilizza il contatto manuale, è importante assicurarsi che tutti i numeri di telefono associati all'account siano sempre aggiornati. Il mancato aggiornamento delle informazioni di contatto potrebbe comportare l'impossibilità di accedere al portale clienti e alla VPN quando PhoneFactor è attivo. Una volta che PhoneFactor è stato aggiunto correttamente, riceverai un'e-mail di conferma. Dopo aver ricevuto l'e-mail, utilizza la seguente procedura per attivare l'autenticazione PhoneFactor.

1. Accedi al portale clienti utilizzando le tue credenziali univoche.
2. Seleziona **Account > Utenti** dalla barra di navigazione.
3. Fai clic sul nome utente per accedere al profilo associato a tale utente.
4. Scorri fino alla sezione **Impostazioni PhoneFactor**.

  Se la sezione Impostazioni PhoneFactor non è disponibile, verifica innanzitutto di aver ricevuto l'e-mail di provisioning di PhoneFactor che indica che PhoneFactor è stato fornito. Se il provisioning di PhoneFactor è stato eseguito ma la sezione non è disponibile, crea un ticket di supporto. Se il provisioning di PhoneFactor non è stato ancora eseguito, attendi l'e-mail e prova di nuovo.
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

Dopo l'attivazione di PhoneFactor, l'autenticazione tramite PhoneFactor è richiesta dal portale clienti o VPN. Dopo l'autenticazione con le credenziali dell'utente, un messaggio ti indica che si sta tentando l'autenticazione PhoneFactor. È necessario che tu, o l'utente che stai aggiungendo, sia vicino al telefono elencato con PhoneFactor per completare l'autenticazione. PhoneFactor tenta l'autenticazione cinque volte. Dopo cinque tentativi di autenticazione non riusciti, verrai bloccato per circa un'ora. Tu o un utente con accesso amministrativo all'account potete modificare le impostazioni di autenticazione PhoneFactor in qualsiasi momento.  Tu o un amministratore dell'account potete disattivare PhoneFactor in qualsiasi momento.

 Se scegli di configurare PhoneFactor per il portale clienti e il tuo accesso VPN, la 2FA per ognuno di essi è separata.
 {: tip}

#### Metodi di autenticazione PhoneFactor
{: #cp_phonefacauthmeths}

Se configuri PhoneFactor come tipo di autenticazione, puoi scegliere una delle seguenti opzioni come metodo di autenticazione:

<dl>
<dt>Telefonata e standard (senza pin)</dt>
<dd>Con questa opzione abilitata, quando accedi al portale, ricevi una chiamata al numero principale abilitato. Quando rispondi alla chiamata, ti viene richiesto di premere il tasto # per completare l'autenticazione.</dd>
<dt>Telefonata con pin</dt>
<dd>Con questa opzione selezionata, immetti un valore pin nel portale clienti. Il pin deve essere compreso tra 4 e 8 numeri. Quando tenti di accedere al portale, ricevi una chiamata al numero principale elencato nel portale. Quando rispondi, ti viene indicato di immettere il tuo numero pin seguito dal simbolo # per completare l'autenticazione.</dd>
<dt>Testo SMS e pin monouso</dt>
<dd>Con questa opzione selezionata, ricevi un messaggio di testo con un pin che utilizzi per rispondere al messaggio. Quando immetti il pin fornito, il processo di autenticazione viene completato e puoi accedere al portale.</dd>
<dt>Testo SMS con monouso e valore pin</dt>
<dd>Con questa opzione selezionata, crea un valore di pin da 4 a 8 numeri. Riceverai quindi un messaggio di testo e risponderai con il codice fornito e il tuo numero pin senza spazi.</dd>
<dt>Applicazione PhoneFactor e standard (senza pin)</dt>
<dd>Apri l'applicazione PhoneFactor (Microsoft Authenticator) sul tuo dispositivo e fai clic su <strong>Autentica</strong>. Verrà visualizzato che sei stato autenticato correttamente utilizzando PhoneFactor e potrai accedere al portale.</dd>
<dt>Applicazione PhoneFactor con pin</dt>
<dd>Con questa opzione, imposta un pin, compreso tra 4 e 8 numeri, nel portale. Viene quindi visualizzata l'applicazione PhoneFactor (Microsoft Authenticator) sul tuo dispositivo. Successivamente, immetti il tuo pin creato nel portale e fai clic su <strong>Autentica</strong> per accedere al portale.</dd>
</dl>
