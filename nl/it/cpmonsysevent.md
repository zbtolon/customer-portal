---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# Monitoraggio degli eventi di sistema dell'infrastruttura {{site.data.keyword.Bluemix_notm}}
{: #customerportal_monevent}

Puoi monitorare gli eventi di sistema per la corretta esecuzione dei tuoi sistemi.  Per informazioni sulla configurazione e gestione dei server virtuali nell'infrastruttura {{site.data.keyword.BluSoftlayer_full}}, vedi [Introduzione ai server virtuali](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers).
{:shortdesc}

## Visualizzazione dei log di controllo per un account
{: #cp_viewacctauditlog}

Ogni account del portale del cliente viene fornito con un log di controllo che tiene traccia delle interazioni di ciascun utente all'interno del portale. Le interazioni tracciate comprendono tentativi di accesso (riusciti e non riusciti), aggiornamenti della velocità della porta, accensione o spegnimento e riavvii nonché le interazioni effettuate dal personale di supporto dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Utilizza la seguente procedura per visualizzare un log di controllo per un account utente.

1. Accedi al [portale del cliente ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Gestisci** > **Log di controllo** dalla barra di navigazione per accedere al log di controllo.

Il log di controllo visualizza inizialmente le ultime 25 interazioni effettuate dagli utenti nell'account. Puoi visualizzare fino a 200 interazioni in qualsiasi momento. Aggiorna il numero di risultati visusalizzati dall'elenco a discesa **Visualizza**. Se le impostazioni sono state modificate, la colonna **Azione** relativa all'interazione conterrà un link. Fai clic su un link per visualizzare l'impostazione interessata dall'azione e i dettagli sulla modifica. Facendo clic sul nome del dispositivo o sul nome utente per una qualsiasi interazione, verrai reindirizzato rispettivamente alla schermata dei dettagli del dispositivo o alla schermata del profilo utente.

## Visualizzazione dei log di accesso per un utente
{: #cp_viewuserlogs}

I log di accesso visualizzano i dati per ciascun tentativo di accesso effettuato da un utente specifico del portale del cliente. I log visualizzano un indicatore di data e ora e l'indirizzo IP per ogni tentativo di accesso. Utilizza la seguente procedura per visualizzare i log di accesso di un utente.

1. Accedi al [portale del cliente ![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Utenti** dalla barra dei menu per accedere alla finestra Utenti.
3. Dall'elenco a discesa **Azioni**, seleziona **Visualizza log di controllo** per visualizzare il log di accesso dell'utente.

Il log di accesso per ciascun utente visualizza i tentativi di accesso effettuati da tale utente per data, insieme all'indirizzo IP da cui è stato effettuato il tentativo. Le informazioni contenute nel log di accesso sono di sola lettura, pertanto non è possibile apportare modifiche al contenuto. Puoi visualizzare nuovamente i log di accesso in qualsiasi momento ripetendo i passi precedenti. Per uscire dai log e tornare alla schermata Utenti, fai clic sul link **Visualizza tutti gli utenti** nella parte superiore della schermata.
