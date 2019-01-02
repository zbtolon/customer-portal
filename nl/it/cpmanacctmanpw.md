---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestione delle password
{: #customerportal_manpws}

Se sei un utente master o il proprietario di un account, puoi abilitare il tracciamento delle password e puoi anche impostare una password per l'accesso una tantum all'account. Il tracciamento delle password consente agli utenti di memorizzare i dati della password del software per i dispositivi e il software associato.
{:shortdesc}

## Abilitazione del tracciamento delle password
{: #customerportal_enabpwtrak}

Il portale clienti ha uno strumento di [tracciamento delle password ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/devices/passwords){:new_window} facoltativo per ogni account. Gli utenti possono recuperare i loro nomi utente e password attraverso lo strumento se le informazioni vengono perse o dimenticate.

I team di supporto utilizzano il tracciamento delle password anche se è richiesto l'accesso remoto a un sistema. I nomi utente e le password vengono utilizzati dal Supporto solo se necessario e autorizzato per la risoluzione del ticket.

Il tracciamento delle password all'interno del portale clienti è facoltativo. Qualsiasi utente con le autorizzazioni appropriate può visualizzare tutte le password memorizzate da questo strumento. Le informazioni su utente e password vengono tracciate manualmente e pertanto non vengono sincronizzate automaticamente con un dispositivo o il suo software. Pertanto, assicurati di aggiornare lo strumento di tracciamento delle password nello stesso momento in cui aggiorni utenti e password su dispositivi e software. Utilizza la seguente procedura per aggiungere un utente allo strumento di tracciamento delle password.

1. Accedi al portale clienti utilizzando le tue credenziali univoche.
2. Seleziona **Dispositivi** > **Gestisci** > **Password** dal menu.
3. Fai clic sulla scheda **Aggiungi credenziali**.
4. Seleziona il **Nome dispositivo** a cui è associato l'utente dall'elenco a discesa **Nome dispositivo**.
5. Seleziona il **Software** a cui è associato l'utente dall'elenco **Software**.

  Il software elencato è fornito dall'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} tramite sottoscrizioni a pagamento o gratuite. Nessun software di terze parti che è stato installato manualmente sul dispositivo è disponibile per il tracciamento attraverso il portale clienti.
  {: tip}

6. Immetti il nome utente e la password per il software nei campi corrispondenti.
8. Facoltativamente, puoi immettere tutti i commenti applicabili nel campo **Note**.
9. Fai clic su **Aggiungi credenziali**.

Dopo aver aggiunto l'utente allo strumento di tracciamento delle password, le informazioni sono memorizzate nello strumento finché non vengono eliminate manualmente. Tutte le combinazioni di nome utente e password vengono memorizzate in base nome del dispositivo per impostazione predefinita. Le voci sono visualizzate in ordine alfabetico per nome dispositivo e quindi per nome utente.

### Filtraggio delle informazioni nello strumento di tracciamento delle password
{: #cp_filterusinfopwtracktool}

Per visualizzare, modificare o eliminare le informazioni utente nello strumento di tracciamento delle password, puoi filtrare per individuare rapidamente un utente. L'utilizzo del filtro per trovare un utente è utile quando l'elenco di utenti si estende su più righe o pagine. Utilizza la seguente procedura per filtrare in base a dispositivo, software o utente nello strumento di tracciamento delle password.

1. Accedi al portale clienti utilizzando le tue credenziali univoche.
2. Seleziona **Dispositivi** > **Gestisci** > **Password** dal menu.
3. Fai clic sulla scheda **Filtro**.
4. Seleziona o immetti il nome dispositivo, software o utente nei campi corrispondenti.
5. Fai clic su **Filtro**.

Puoi selezionare le informazioni utente da visualizzare, modificare o rimuovere.

### Modifica delle informazioni utente nello strumento di tracciamento delle password
{: #cp_editusinfopwtracktool}

Dopo aver aggiunto un utente allo strumento di tracciamento delle password, puoi modificare i dettagli associati all'utente o alla password. Utilizza la seguente procedura per modificare le informazioni per un utente nello strumento di tracciamento delle password.

1. Accedi al portale clienti utilizzando le tue credenziali univoche.
2. Seleziona **Dispositivi** > **Gestisci** > **Password** dal menu.
3. Individua la combinazione dispositivo-utente nello strumento. Utilizza la funzione di filtro per individuare rapidamente un utente.
4. Fai clic in qualsiasi punto della riga per aprire la vista dei dettagli dell'utente.
5. Aggiorna i campi **Nome utente** o **Password** secondo necessità.
6. Fai clic su **Aggiorna** per salvare le modifiche.

Dopo aver modificato un utente o una password nello strumento di tracciamento delle password, le informazioni vengono aggiornate immediatamente.

## Configurazione di un account per l'accesso con password monouso
{: #cp_confportacc1timpwacc}

Prima di poter configurare l'account, devi configurare l'applicazione "VIP Access" di Verisign. Se VIP Access non è configurato, per prima cosa scarica l'applicazione per uno dei seguenti dispositivi:
* Per il tuo telefono: [https://m.vip.symantec.com/home.v ![Icona link esterno](../icons/launch-glyph.svg)](https://m.vip.symantec.com/home.v){:new_window}
* Per il tuo desktop:  [https://idprotect.verisign.com/desktop/download.v ![Icona link esterno](../icons/launch-glyph.svg)](https://idprotect.verisign.com/desktop/download.v){:new_window}

Completa quindi la seguente procedura:
1. Apri l'applicazione. Trova l'ID credenziale e la tua password monouso corrente. Inizialmente puoi ignorare la password ma ti servirà l'ID credenziale per il portale, quindi mantieni aperta l'applicazione.
2. Accedi al portale clienti come utente per il quale vuoi configurare la password monouso.
3. Fai clic su **Account** > **Users** > **Actions** > **Add External Authentication**.
4. Seleziona il tipo di autenticazione da aggiungere. Se stai utilizzando l'applicazione Verisign, scegli **Symantect Identity Protection**.
5. Immetti l'ID credenziale dal passo 1 e fai clic su **Continue**.
6. Completa il processo di ordinazione e l'opzione di sicurezza aggiuntiva viene applicata automaticamente in pochi minuti.
7. Dopo alcuni minuti, fai clic su **Account** > **Users** dalla barra di navigazione e seleziona l'utente per il quale hai configurato la password monouso.
8. Fai clic sul link **Update Credential** nella sezione **Symantec Validation Settings**.
9. Seleziona **enabled** per lo **Credential State** e fai clic su **Update credential**.
10. Una volta che l'opzione di sicurezza aggiuntiva è stata elaborata correttamente, puoi accedere al portale clienti come al solito. Dopo aver inserito il nome utente e la password, ti viene richiesto di immettere un codice di sicurezza.
11. Apri l'applicazione Verisign Identity Protection sul tuo dispositivo preferito e fornisce il codice che viene visualizzato per accedere.

Salva il tuo ID credenziale originale di Verisign Identity Protection in un luogo sicuro per riferimenti futuri. Senza di questo, non puoi accedere al portale.

## Reimpostazione della password
{: #cp_reset-your-password}

La reimpostazione della tua password si basa sulla possibilità di utilizzare un ID IBM per l'autenticazione per accedere al tuo account.  

### Reimpostazione di una password dell'account ID IBM
{: #cp_reset-IBMid-password}

Se utilizzi l'ID IBM per l'autenticazione, per reimpostare o ripristinare la tua password vai al tuo profilo ID IBM e segui le istruzioni nella sezione **Accedi**.

### Reimpostazione di una password dell'account SoftLayer
{: #cp_reset-password}

Se non utilizzi un ID IBM per l'autenticazione dell'account, completa la seguente procedura:

1. Fai clic sul link della password persa nella pagina di accesso del [portale clienti ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}.
2. Quando ti viene richiesto, immetti il tuo nome utente corrente.
3. Controlla la tua email per trovare una nota con un link per reimpostare la password. Questo link è valido per 24 ore.
4. Seleziona e rispondi alle tre domande di sicurezza.

Hai 5 tentativi per rispondere alle domande di sicurezza. Se effettui più di 5 tentativi, il modulo di reimpostazione della password viene bloccato per 15 minuti prima che puoi riprovare.

Per informazioni sull'utilizzo delle password VPN, consulta [Aggiorna una password VPN dell'utente](/docs/infrastructure/iaas-vpn/update-password.html#update-a-user-s-vpn-password).
{: tip}
