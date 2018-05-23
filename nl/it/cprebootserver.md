---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-05"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Riavvio del tuo server
{: #customerportal_rebootserver}

A volte, nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} si verificano degli eventi che richiedono il riavvio del server.
{:shortdesc}

Utilizza la seguente procedura per riavviare il tuo server:
1. Dal portale clienti, fai clic sulla scheda **Supporto**.
2. Fai clic su **Riavvia**.
3. Seleziona il server da riavviare e fai clic su **Riavvia**.
4. Seleziona uno dei seguenti metodi per riavviare il server:
  * Predefinito (tentare il riavvio con IPMI e quindi con il filo dell'alimentazione)
  * IPMI
  * Filo dell'alimentazione
5. Fai clic su Riavvia.

Questa pagina offre anche la possibilità di eseguire l'avvio nel kernel di salvataggio, che è molto utile se si verifica un problema in cui il server non può avviare il sistema operativo a causa di un problema di configurazione. Dopo l'avvio nel kernel di salvataggio, puoi montare l'unità o le unità del tue server e quindi correggere il problema di configurazione. Una volta corretto il problema, puoi riavviare il server dalla riga di comando e il server verrà riavviato nel kernel predefinito per il tuo server. Dopo aver eseguito il comando di riavvio, visualizzerai un tempo stimato per il completamento.
