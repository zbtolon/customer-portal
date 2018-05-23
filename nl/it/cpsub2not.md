---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Sottoscrizione alle notifiche
{: #cp_bpnotifications}

A volte, nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} si verificano degli eventi che richiedono un'azione; alcuni sono inaspettati mentre altri sono delle attività di manutenzione pianificata necessarie per mantenere il funzionamento dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} in condizioni ottimali. I clienti vengono isolati da questi eventi il più possibile, ma a volte è necessario portare offline le attrezzature. Indipendentemente dall'impatto sui clienti, è sempre necessario essere trasparenti, tempestivi e informativi.
{:shortdesc}

Perché tu debba avere il controllo della tua esperienza nel cloud, hai bisogno di informazioni tempestive sulle attività di manutenzione. Per ottenere queste informazioni, puoi sottoscrivere alle notifiche dal portale clienti. L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} utilizza il processo di notifica EMS (Event Management System) per i seguenti tipi di eventi operativi importanti:
* Problemi di infrastruttura non pianificati: problemi che potrebbero causare un'interruzione in determinate condizioni per clienti specifici
* Manutenzione del servizio pianificata: manutenzione necessaria per mantenere l'infrastruttura operativa in uno stato ottimale
* Ticket di supporto aperti: avvisa gli utenti sottoscritti in merito ai ticket aperti sul loro account

Le notifiche dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} sono state progettate per gli ambienti cloud aderendo ai seguenti principi chiave:
* Automatizzate attraverso il portale clienti
* Scalabili per raggiungere una community ampia e in crescita
* Mirate a consentire all'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} di identificare solo i clienti e il sottoinsieme di risorse interessati dall'evento.

Affinché il sistema di notifica sia pienamente efficace, sottoscrivi il processo. Se hai un ambiente critico che lo richiede, stabilisci anche una copertura di 24 ore.

Per una panoramica di come vengono fornite le notifiche dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}, vedi [Improving communications for customer-affecting planned events ![Icona link esterno](../icons/launch-glyph.svg)](http://blog.softlayer.com/2014/improving-communications-customer-affecting-planned-events){:new_window}.

## Politica dell'intervallo di notifica
{: #cp_bpgsnotiftimpol}

Il tempo di preavviso che l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} dà agli utenti prima dell'evento in sospeso varia a seconda che l'evento sia un problema di infrastruttura non pianificato o una manutenzione pianificata o programmata. In generale, la politica dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} è di porre rimedio ai problemi il più rapidamente possibile per rimuovere o ridurre al minimo il rischio di ulteriori sviluppi di problemi che potrebbero avere un impatto maggiore. Ciò significa che a volte anche la manutenzione pianificata viene eseguita solo con breve preavviso.

### Panoramica della politica
{: #cp_bpgsnotifpolover}

Ti vengono notificati i seguenti tipi di interruzioni o problemi come descritto in ogni sezione.

#### Problemi o interruzioni non pianificati
L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} comunica il più rapidamente possibile ai clienti interessati le informazioni relative allo scopo dell'infrastruttura, alle soluzioni alternative o alle stime di risoluzione non appena tali informazioni sono note. La comunicazione tempestiva ti fornisce le informazioni necessarie per pianificare gli imprevisti e garantisce che l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} stia affrontando il problema.

#### Manutenzione pianificata
L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} fornisce una notifica per la manutenzione pianificata prima dell'evento. Ci sono delle volte in cui la manutenzione dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} è un'emergenza, che potrebbe comportare un preavviso più breve. L'obiettivo è sempre quello di trovare l'equilibrio ideale tra fornire una quantità ragionevole di preavviso per permetterti di pianificare gli imprevisti e aggiornare o migliorare l'infrastruttura che tipicamente porta a miglioramenti alla stabilità generale o all'aggiunta delle funzionalità necessarie.

#### Vulnerabilità di sicurezza
L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} isola l'area interessata, crea una patch per chiudere la vulnerabilità e testa la patch per garantire che nessuna funzione collaterale venga influenzata. Spesso, questo lavoro viene svolto con un altro fornitore che potrebbe fornire parti della tecnologia interessata. Di solito c'è un embargo di notifica pubblica per le patch di sicurezza, che vengono mantenute poco per proteggere il pubblico, ma ciò richiede un periodo di preavviso più breve. L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} implementa le patch in tutta infrastruttura interessata prima che il pubblico venga informato del problema, il che altrimenti aumenterebbe il rischio. Più velocemente la vulnerabilità viene chiusa, prima viene rimosso il rischio, il che significa che i problemi di sicurezza richiedono una breve finestra di notifica.

Uno degli obiettivi più frequenti per le violazioni della sicurezza è il software di infrastruttura virtuale. L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} utilizza popolari tecnologie open source e dei partner per offrire la propria offerta di Virtual Server. Per implementare una correzione di sicurezza, i server dei clienti che eseguono software di infrastruttura virtuale potrebbero dover essere portati offline per applicare patch e riavviare l'ambiente, causando delle interruzioni. Per ridurre al minimo l'impatto sui clienti, l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} ha recentemente implementato un miglioramento del processo di notifica per l'infrastruttura virtuale: comunicazioni migliorate. I clienti ricevono una notifica con un'ora di inizio specifica e una finestra di 90 minuti per ciascun pod, il che si traduce in tempi di interruzione più brevi e tempistiche più accurate che aiutano a prepararti meglio. Il sistema di notifica isola la manutenzione per ciascun account, consentendo all'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} di informare i clienti non appena i loro host specifici vengono serviti, il che avviene molto spesso prima della finestra di 90 minuti.

#### Più POD o data center interessati
L'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} si sforza di dare un preavviso più lungo, a meno che non vi sia un'urgenza estrema di implementare la correzione per evitare un impatto secondario ancora maggiore.


## Aggiunta di sottoscrittori alle notifiche evento
{: #cp_bpaddsub2eventnotcp}

Sempre più spesso, i clienti IBM si affidano ai servizi dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} (IaaS), contrattando con IBM per i servizi di infrastruttura gestita, contrattando per servizi cloud eseguiti sull'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} o contrattando direttamente con i servizi dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Quando i servizi cloud coinvolgono l'infrastruttura, solo gli utenti dell'account SoftLayer sono autorizzati a ricevere notifiche, come descritto nella sezione precedente. In alcuni casi, potresti non volere che i team degli account o dei servizi gestiti IBM siano coinvolti nelle operazioni o che il supporto dei servizi di infrastruttura accedano ai tuoi account SoftLayer. Nel portale clienti dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} è stata aggiunta una nuova funzione che ti consente di designare un elenco di sottoscrittori, ad esempio il personale IBM, per ricevere notifiche senza privilegi sui tuoi account.

Per designare un elenco di sottoscrittori, gli utenti master possono accedere al proprio account del portale clienti e utilizzare la seguente procedura:
1. Fai clic su su **Account** > **Gestisci** > **Sottoscrizioni** dal menu.
2. Scegli il tipo di evento a cui aggiungere i sottoscrittori.
2. Dalla finestra a comparsa, aggiungi uno o più indirizzi e-mail. Gli indirizzi e-mail possono essere IBM o non IBM.
3. Fai clic su **Crea**.

Gli indirizzi e-mail aggiunti come sottoscrittori supplementari ricevono notifiche di eventi pianificati e non pianificati e ticket di supporto aperti. Le notifiche contengono dettagli tecnici quindi devi tenerne conto quando aggiungi i sottoscrittori. A causa della natura tecnica dettagliata delle notifiche, i sottoscrittori previsti sono coloro che possono comprendere, in dettaglio, in che modo la notifica influisce sul tuo ambiente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}. Sottoscrivere destinatari che non siano in grado di comprendere l'impatto potenziale del client sulla base dei dettagli nella notifica è controproducente e fortemente sconsigliato.
