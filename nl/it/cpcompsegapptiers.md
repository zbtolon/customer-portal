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

# Protezione e ridimensionamento del tuo ambiente
{: #cp_compsegapptierssecscal}

Quando ospiti un'applicazione, due degli aspetti più importanti che qualsiasi amministratore di sistema deve considerare sono la sicurezza e la scalabilità dell'applicazione.
{:shortdesc}

## Protezione dei tuoi sistemi con i firewall
{: #cp_bpsecuresystem}

Utilizza i firewall hardware disponibili per assicurarti che il tuo dispositivo sia sempre sicuro. Puoi eseguire il provisioning di firewall hardware su richiesta senza tempi di inattività, se vengono stabilite correttamente delle regole, per proteggere il tuo server da attività indesiderate.

I firewall sono servizi aggiuntivi per qualsiasi dispositivo che devi configurare e abilitare manualmente per garantirne l'efficacia. Puoi bloccare porte superflue e disabilitare le porte pubbliche per sistemi basati su reti private per gestire ulteriormente l'accessibilità esterna ai tuoi sistemi. Le regolari scansioni delle vulnerabilità nel portale clienti identificano eventuali rischi di sicurezza in sospeso o sconosciuti in modo da poter ridurre rapidamente tali rischi.

Dopo aver ordinato il firewall, è necessario abilitarlo e impostare le regole.

### Attivazione del firewall
{: #cp_bpnofirewalbypass}

L'acquisto di un firewall è il primo passo per proteggere i tuoi sistemi, ma il semplice acquisto di un firewall non consente di proteggerti. Dopo il provisioning, il tuo firewall è in **modalità Bypass** e non ha alcuna regola impostata. Per rendere operativo il tuo firewall, devi creare delle regole e attivare il firewall in modo che possa iniziare a bloccare attività indesiderate.


## Protezione del tuo ambiente segmentando i livelli dell'applicazione
{: #cp_copmsecenv}

Segmentando i livelli di applicazione logica in livelli di infrastruttura fisica, puoi fornire una maggiore sicurezza utilizzando gli elenchi di controllo accesso (ACL). Quando segmenti i livelli di applicazione, uno dei componenti più importanti da considerare è il tipo di traffico da consentire in ogni livello e da dove. Per determinare queste informazioni, pensa a come funziona fondamentalmente la tua applicazione e a quali servizi si supportano reciprocamente per fornire agli utenti il contenuto che hanno richiesto.

Ad esempio, considera un'applicazione a due livelli che si basa su un front-end web e un back-end del database. Per questa applicazione, assicurati che le porte 80 e 443 (se stai usando SSL) siano aperte su Internet sui tuoi server web. Probabilmente vuoi anche bloccare tutte le porte su Internet e gestire il tuo server tramite VPN utilizzando la rete privata dell'infrastruttura {{site.data.keyword.BluSoftlayer_full}}. È probabile che tu voglia anche annullare il bind dell'indirizzo IP pubblico sul tuo server di database e trasmettere ad esso tutto il traffico attraverso la porta 1433 (per MSSQL) o la porta 3306 (per {{site.data.keyword.mysql}}) dal tuo server web. Potresti gestire il tuo server di database sulla rete privata proprio come il tuo server web. Potresti inoltre configurare un firewall software sul server di database per bloccare tutto il traffico dal server web alle specifiche porte del database.

Configurando il tuo ambiente in questo modo, impedendo l'accesso a SSH o RDP da Internet e disabilitando tutto il traffico Internet nel tuo database, aumenti la sicurezza. La creazione di ACL tra il livello web e il livello del database rende più difficile danneggiare il tuo database se il server web viene compromesso.

## Ridimensionamento del tuo ambiente segmentando i livelli dell'applicazione
{: #cp_copmscaleenv}

Un ambiente multilivello offre anche facilità di scalabilità rispetto alle architetture verticali o ad host singolo. Puoi configurare un ambiente multilivello per semplificare il ridimensionamento incrementale della tua applicazione, consentendo il ridimensionamento per i servizi che richiedono più risorse. Ad esempio, nello scenario precedente, se il tuo server web è sottoposto a tassazione eccessiva, puoi distribuire un altro server web. Puoi quindi replicare i dati del sito o dell'applicazione e bilanciare il carico o configurare il DNS round robin per consentire ai tuoi due server web di suddividere il carico web. Il DNS round robin o il bilanciamento del carico forniscono un'elevata disponibilità al tuo ambiente, consentendo a più server web di rispondere alle richieste in entrata. Se un singolo server si interrompe, è disponibile un altro nodo per gestire le richieste dell'utente.

Puoi anche eseguire il ridimensionamento incrementale del tuo database. Ad esempio, con un database {{site.data.keyword.mysql}}, un'opzione è quella di configurare un altro server fisico e utilizzarlo come subordinato in una configurazione di replica {{site.data.keyword.mysql}}. Puoi segmentare tutte le scritture del database sul master e tutte le letture su uno o più subordinati per ridimensionare il database in modo da supportare più carico. Questo tipo di configurazione aggiunge anche un livello di alta disponibilità in quanto puoi modificare lo stato di un subordinato in master. Puoi quindi instradare sia il traffico di lettura che quello di scrittura al subordinato se il tuo nodo master {{site.data.keyword.mysql}} viene interrotto.

Queste idee sono solo alcuni dei molti modi per proteggere e ridimensionare il tuo ambiente. Se hai domande o dubbi relativi al modo migliore di progettare il tuo ambiente da un punto di vista della sicurezza o della scalabilità, l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} ha un team Sales Engineering che può aiutarti.
