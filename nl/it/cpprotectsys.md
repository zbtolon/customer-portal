---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-16"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Protezione dei sistemi
{: #customerportal_protsys}

La protezione dei sistemi garantisce che i tuoi sistemi funzionino in modo scorrevole e senza inutili interruzioni.

## Utilizza la rete privata
{: #cp_bpuseprivnet}

Puoi gestire i tuoi dispositivi in un ambiente altamente sicuro utilizzando la rete privata dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Quando possibile, interagisci con i tuoi dispositivi utilizzando una connessione VPN e abilita lo spanning della rete in modo che i tuoi sistemi comunichino sulla rete privata. Per accedere alla rete privata, modifica l'accesso VPN dell'utente dall'[Elenco utenti![Icona link esterno](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Utilizza l'elenco [VPN (Virtual Private Network) ![Icona link esterno](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} per la connessione a una delle varie opzioni VPN.

### Non lasciare le porte RDP, SSH o di controllo sulla rete pubblica
{: #cp_bpnordpsshcponpubnet}

La rete pubblica è ottima per molte cose, ma ci sono alcuni aspetti che, se lasciati disponibili sulla rete pubblica attraverso delle porte aperte, possono rendere il tuo sistema vulnerabile. Proteggiti disabilitando RDP o limitando SSH sulla rete pubblica. Se questi servizi devono essere disponibili sulla rete pubblica, valuta lo spostamento di RDP o SSH a un numero di porta personalizzato.

## Proteggi i tuoi dati attraverso backup regolari
{: #cp_bpsafedataregback}

Pianifica i backup per garantire che i tuoi dati siano memorizzati in modo sicuro al di fuori del tuo dispositivo e riuscire a ricaricarli se vengono persi.

L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} offre più soluzioni di backup per garantirti di poter recuperare i dati in caso di errore dell'unità o di errore dell'utente. Le soluzioni di backup attualmente includono NAS, EVault Backup e R1Soft CDP, che sono tutti disponibili in una varietà di opzioni di archiviazione.
Ad esempio, puoi scegliere uno dei seguenti servizi di backup per memorizzare i dati in un luogo sicuro: 
  * EVault Backup è un sistema di backup automatizzato basato sull'agent. Questa è una comune soluzione “set-and-forget” (imposta e dimentica) per la gestione del tuo dispositivo. È compatibile con i software Microsoft tra cui Exchange e SQL tramite plug-in aggiuntivi. Gli utenti EVault interagiscono con questo servizio tramite l'applicazione basata sul web WebCC di EVault.
  * R1Soft Continuous Data Protection (CDP) può essere installato sul tuo server o sulla macchina virtuale autogestita. È consigliabile se desideri una singola interfaccia per gestire tutti i backup. Interagisci con R1Soft CDP tramite il tuo sistema di gestione proprietario, che consente di installare gli agent su macchine virtuali e offre plug-in di database per funzionalità aggiuntive.

 Consulta la pagina [Storage ![Icona link esterno](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} per ulteriori informazioni su ciascuna soluzione di backup e vedi [Introduzione ai servizi di backup](/docs/infrastructure/Backup/index.html) per ulteriori informazioni sul backup dei tuoi dati.

### Non supporre di avere ridondanza, sai di averla
{: #cp_bpknowredundant}

L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} offre molteplici ridondanze aggiuntive, inclusi alimentatori ridondanti a doppio percorso e configurazioni RAID. Verifica di aver eseguito il provisioning di una o più di queste funzioni per assicurarti di lavorare in un ambiente ridondante e di essere protetto in caso di errore.

### Conferma di aver eseguito il backup delle tue informazioni prima di effettuare un ricaricamento SO
{: #cp_bpnoperfOSwobackupconf}

Il ricaricamento del sistema operativo rimuove tutti i dati dal disco rigido del dispositivo. Prima di avviare il ricaricamento SO, esegui il backup delle informazioni e verifica l'esito positivo di tale backup in modo che nessuna informazione venga persa. Una volta completato il ricaricamento SO, le informazioni perse non possono essere recuperate.

## Non rimuovere ASM (Adaptec Storage Manager)
{: #cp_bpsupdontremovasm}

 L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} utilizza ASM per monitorare lo stato del tuo array RAID. Se elimini questo software, il team di supporto non può monitorare il tuo dispositivo. Se ASM viene rimosso dal dispositivo, gli avvisi di errore RAID non sono disponibili e non ti viene notificato l'errore tramite il sistema di notifica automatico.
