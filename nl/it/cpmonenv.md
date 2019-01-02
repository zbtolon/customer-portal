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


# Monitoraggio dell'ambiente e degli eventi di sistema
{: #customerportal_cpmonenvsysevent}

Monitoraggio dell'ambiente significa che hai la possibilità di controllare i dispositivi in qualsiasi momento e che ricevi automaticamente una notifica in caso di interruzione di uno dei tuoi dispositivi. Puoi anche monitorare gli eventi di sistema per la corretta esecuzione dei tuoi sistemi.  
{: shortdesc}

## Monitoraggio dell'ambiente
{: #cpmonenv}

Come minimo, utilizza il monitoraggio ping di base, ma puoi personalizzare le opzioni di monitoraggio adeguandole alle tue esigenze di business.

### Resta informato sugli eventi di manutenzione della rete e sugli eventi non pianificati
{: #cp_stayinfomaintevent}

Di tanto in tanto, la manutenzione pianificata e di emergenza della rete è inevitabile. L'infrastruttura {{site.data.keyword.BluSoftlayer_full}} mantiene molti canali per tenerti informato su tutti gli eventi di manutenzione pianificata e di emergenza. Inoltre, puoi [sottoscrivere alle notifiche e-mail](/docs/customer-portal/cpsub2not.html) dal sistema di gestione eventi (EMS o Event Management System). Questo servizio gratuito invia automaticamente agli utenti sottoscritti email riguardanti gli eventi non pianificati, che potrebbero influire sui servizi.

### Utilizzo dell'applicazione mobile dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}
{: #cp_bmxinframobile}

Utilizza l'applicazione mobile dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} per gestire i dispositivi dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} mentre sei in movimento utilizzando il tuo dispositivo mobile iOS o Android. Le funzionalità all'interno dell'applicazione mobile dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} comprendono il supporto dei ticket, il controllo di base dei dispositivi e il monitoraggio della larghezza di banda.

L'applicazione mobile dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} integra la funzionalità del portale clienti in quanto puoi monitorare le informazioni critiche sulla tua infrastruttura da qualsiasi luogo utilizzando il dispositivo mobile connesso alla rete. L'applicazione si evolve in modo rapido e vengono aggiunte regolarmente nuove funzionalità, ma puoi utilizzare l'applicazione mobile per eseguire attività come le seguenti:
  * Visualizzare, creare e aggiornare i ticket di supporto
  * Monitorare lo stato del dispositivo, incluso la larghezza di banda e gli allarmi
  * Arrestare e riavviare i Bare Metal Server e i server virtuali
  * Visualizzare le fatture degli account ed effettuare pagamenti una tantum
  * Accedere ed esaminare i contenuti memorizzati in Object Storage

L'applicazione mobile dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} è utilizzabile su diverse piattaforme per dispositivi mobili popolari ed è disponibile gratuitamente dai relativi application store per ciascuna piattaforma.

## Monitoraggio dei server
{: #customerportal_monservers}

Configura il monitoraggio per controllare lo stato del tuo server e sapere quando ridimensionare. Puoi utilizzare il monitoraggio standard o i servizi di monitoraggio Nimsoft. Puoi utilizzare il monitoraggio standard, o di base, nel metodo ping-and-respond (effettua ping e rispondi) utilizzando un ping lento o di servizio dal portale clienti dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Puoi anche utilizzare il monitoraggio Nimsoft, o avanzato, dal portale clienti o in 1 di 3 livelli: base, avanzato e premium. Per ulteriori informazioni specifiche per i server bare metal, vedi [Introduzione ai server bare metal](/docs/bare-metal/index.html#getting-started).

## Monitoraggio degli eventi di sistema
{: #customerportal_monevent}

Puoi monitorare gli eventi di sistema visualizzando i log di controllo e i log di accesso.

### Visualizzazione dei log di controllo per un account
{: #cp_viewacctauditlog}

Ogni account del portale clienti viene fornito con un log di controllo che tiene traccia delle interazioni di ciascun utente all'interno del portale. Ad esempio, vengono tracciate le seguenti interazioni:
  * Tentativi di accesso (riusciti e non riusciti)
  * Aggiornamenti della velocità della porta
  * Accensione o spegnimento e riavvii
  * Interazioni effettuate dal personale di supporto dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.

Utilizza la seguente procedura per visualizzare un log di controllo per un account utente.

1. Accedi al [Portale clienti ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Gestisci** > **Log di controllo** dalla barra di navigazione per accedere al log di controllo.

Il log di controllo visualizza inizialmente le ultime 25 interazioni effettuate dagli utenti nell'account. Puoi visualizzare fino a 200 interazioni in qualsiasi momento. Aggiorna il numero di risultati che vengono visualizzati dall'elenco a discesa **Visualizza**. Se le impostazioni sono state modificate, la colonna **Azione** relativa all'interazione contiene un link. Fai clic su un link per visualizzare l'impostazione interessata dall'azione e i dettagli sulla modifica. Facendo clic sul nome del dispositivo o sul nome utente per una qualsiasi interazione, verrai reindirizzato alla schermata dei dettagli del dispositivo o alla schermata del profilo utente.

### Visualizzazione dei log di accesso per un utente
{: #cp_viewuserlogs}

I log di accesso visualizzano i dati per ciascun tentativo di accesso effettuato da un utente specifico del portale clienti. I log visualizzano un indicatore di data e ora e l'indirizzo IP per ogni tentativo di accesso. Utilizza la seguente procedura per visualizzare i log di accesso di un utente.

1. Accedi al [portale clienti ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Utenti** dalla barra dei menu per accedere alla finestra Utenti.
3. Dall'elenco a discesa **Azioni**, seleziona **Visualizza log di controllo** per visualizzare il log di accesso dell'utente.

Il log di accesso per ciascun utente visualizza i tentativi di accesso effettuati da tale utente per data, insieme all'indirizzo IP da cui è stato effettuato il tentativo. Le informazioni nel log di accesso sono di sola lettura, pertanto non è possibile in alcun momento apportare modifiche al contenuto. Puoi visualizzare nuovamente i log di accesso in qualsiasi momento ripetendo i passi precedenti. Per uscire dai log e tornare alla schermata Utenti, fai clic sul link **Visualizza tutti gli utenti**.
