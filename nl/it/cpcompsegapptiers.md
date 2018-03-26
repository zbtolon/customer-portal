---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Protezione e ridimensionamento del tuo ambiente
{: #cp_compsegapptierssecscal}

Qquando si effettua l'hosting di un'applicazione, an application, due degli aspetti più critici che qualsiasi amministratore di sistema deve considerare sono la sicurezza e la scalabilità dell'applicazione.
{:shortdesc}

## Protezione dei tuoi sistemi con i firewall
{: #cp_bpsecuresystem}

I firewall sono servizi aggiuntivi per qualsiasi dispositivo che devi configurare e abilitare manualmente per garantirne l'efficiacia. Puoi bloccare porte superflue e disabilitare le porte pubbliche per sistemi basati su reti private per gestire ulteriormente l'accessibilità esterna ai tuoi sistemi. L'esecuzione di scansioni regolari delle vulnerabilità nel portale del cliente identifica eventuali rischi di sicurezza rilevanti o sconosciuti in modo da poter ridurre rapidamente tali rischi.

### Attivazione del firewall
{: #cp_bpnofirewalbypass}

L'acquisto di un firewall è il primo passo per proteggere i tuoi sistemi, ma il semplice acquisto di un firewall non consente di proteggerti. Dopo il provisioning, il tuo firewall è in **modalità Bypass** e non ha alcuna regola impostata. Per rendere operativo il tuo firewall, devi creare delle regole e attivare il firewall in modo che possa iniziare a bloccare attività indesiderate.


## Protezione del tuo ambiente segmentando i livelli dell'applicazione
{: #cp_copmsecenv}

Segmentando i livelli di applicazione logica in livelli di infrastruttura fisica, puoi garantire una maggiore sicurezza tramite l'utilizzo di elenchi di controllo degli accessi (ACL). Quando si segmentano i livelli di applicazione, uno dei componenti più importanti da prendere in considerazione è il tipo di traffico da consentire in ogni livello e da dove trasmetterlo. Per determinarlo, devi riflettere su come funziona fondamentalmente la tua applicazione e su quali servizi si supportano reciprocamente per fornire all'utente finale il contenuto richiesto.

Ad esempio, con un'applicazione a due livelli che si basa su un database backend e frontend web, dovrai assicurarti che le porte 80 e 443 (se utilizzi SSL) siano aperte per Internet sui tuoi server web. Probabilmente vorrai anche bloccare tutte le porte su Internet e gestire il tuo server su VPN utilizzando la rete privata dell'infrastruttura {{site.data.keyword.BluSoftlayer_full}}. In questo scenario, potresti voler annullare il bind dell'indirizzo IP pubblico sul tuo server di database e trasmettere ad esso tutto il traffico attraverso la porta 1433 (per MSSQL) o la porta 3306 (per {{site.data.keyword.mysql}}) dal tuo server web.  Il server di database può essere gestito tramite la rete privata proprio come il tuo server web e puoi configurare un firewall software sul server di database per bloccare tutto il traffico dal server web alle porte del database specifiche. 

Configurando il tuo ambiente in questo modo, aumenti la sicurezza impedendo alle persone di accedere a SSH o RDP da Internet e disabilitando tutto il traffico Internet verso il tuo database. La creazione di ACL tra il livello web e livello di database rende più difficile danneggiare il tuo database nel caso in cui il server web venga compromesso. 

## Ridimensionamento del tuo ambiente segmentando i livelli dell'applicazione
{: #cp_copmscaleenv}

Un ambiente multilivello offre anche facilità di scalabilità rispetto alle architetture verticali o ad host singolo. Puoi configurare un ambiente multilivello per semplificare il ridimensionamento incrementale della tua applicazione, consentendo il ridimensionamento per i servizi che richiedono risorse aggiuntive. Ad esempio, nello scenario precedente, se il tuo server web è sottoposto a tassazione eccessiva, puoi semplicemente distribuire un altro server web, replicare i dati del sito o dell'applicazione e configurare il bilanciamento del carico o il DNS round robin per consentire ai tuoi due server web di suddividere il carico web. Il DNS round robin o bilanciamento del carico fornisce un'elevata disponibilità al tuo ambiente, consentendo a più server web di rispondere alle richieste in entrata.  Se un singolo server si interrompe, è disponibile un altro nodo per gestire le richieste dell'utente finale.

Puoi anche eseguire il ridimensionamento incrementale del tuo database. Ad esempio, con un database {{site.data.keyword.mysql}}, un'opzione è quella di configuirare un altro server fisico e utilizzarlo come 'slave' in una configurazione di replica Master/Slave {{site.data.keyword.mysql}}. Puoi segmentare tutte le scritture del database sul 'master' e tutte le letture su uno o più 'slave' per ridimensionare il database per supportare più carico.  Questo tipo di configurazione aggiungerà anche un livello di alta disponibilità consentendoti di modificare lo stato di uno 'slave' in 'master' e instradare ad esso sia il traffico di lettura che di scrittura nel caso in cui il nodo 'master' {{site.data.keyword.mysql}} si interrompa. 

Queste idee sono solo alcuni dei molti modi per proteggere e ridimensionare il tuo ambiente. Se hai domande o dubbi relativi al modo migliore di progettare il tuo ambiente da una prospettiva di sicurezza o scalabilità, l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} ha un team Sales Engineering che può aiutarti.
