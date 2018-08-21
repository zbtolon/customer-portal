---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-15"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Esercitazione introduttiva
{: #getting-started}

In questa esercitazione, illustreremo il processo per rendere operativo il tuo account SoftLayer in modo che tu possa iniziare a ordinare e gestire le tue risorse dell'infrastruttura.
{:shortdesc}

## Prima di iniziare
{: #prereqs}

Hai bisogno di un [account {{site.data.keyword.Bluemix}} ![Icona link esterno](../icons/launch-glyph.svg "Icona link esterno")](https://control.bluemix.net/){:new_window}. Accedi al portale clienti con le tue credenziali dell'ID IBM. La maggior parte dei nuovi utenti utilizza l'[ID IBM ](/docs/account/softlayerlink.html#switchtoIBMid) per l'autenticazione.

Se non utilizzi l'ID IBM per l'autenticazione per accedere al tuo account, esegui l'accesso al portale clienti con le tue credenziali univoche dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.
{: tip}

## Passo 1: configura il tuo account
{: #account-setup}

La configurazione del tuo account include la verifica delle informazioni di contatto e dei dettagli di fatturazione:
 * Per verificare i dettagli di contatto dell'azienda, vai a **Account** > **Gestisci** > **Contatti azienda**. Le informazioni di contatto dell'azienda del tuo account vengono utilizzate per notificare eventuali problemi o modifiche al tuo account.
 * Per verificare i dettagli del profilo dell'azienda, vai a **Account** > **Gestisci** > **Profilo azienda**. Le informazioni del profilo azienda includono dettagli relativi al titolare dell'account principale.
 * Per verificare i dettagli di fatturazione, vai a **Account** > **Fatturazione** > **Metodo di pagamento**. Il metodo di pagamento mensile è la carta di credito che viene fatturata su base ricorrente per i pagamenti associati al tuo account.

## Passo 2: aggiungi utenti e assegna le autorizzazioni
{: #users-permissions}

Per aggiungere utenti al tuo account e impostare le autorizzazioni iniziali, vai a **Account** > **Utenti**.
 * Per invitare gli utenti alle risorse della piattaforma e dell'infrastruttura nel tuo account in base a specifiche autorizzazioni da te assegnate, fai clic su **Invita utenti**. Vieni quindi indirizzato all'interfaccia utente di {{site.data.keyword.Bluemix_notm}} Identity and Access Management (Tivoli Information Archive Manager) per invitare utenti e assegnare l'accesso. Per ulteriori informazioni, vedi [Invito di utenti e assegnazione dell'accesso](/docs/iam/iamuserinv.html).
 * Per aggiungere solo utenti con accesso VPN, fai clic su **Aggiungi utente solo VPN**. Immetti le informazioni personali, imposta le autorizzazioni del portale e imposta l'accesso al dispositivo per l'utente.

Quando imposti le autorizzazioni dell'infrastruttura nell'invito iniziale, puoi scegliere una di tre seri di autorizzazioni: Solo visualizzazione, Utente di base e Super utente. Dopo che gli utenti accettano l'invito, puoi personalizzare il loro accesso modificando le autorizzazioni del portale. Per ulteriori informazioni, vedi [Autorizzazioni dell'infrastruttura](/docs/iam/infrastructureaccess.html).
{: tip}

## Passo 3: abilita l'accesso alla rete privata dell'infrastruttura {{site.data.keyword.Bluemix_notm}}
{: #enable-private-network}

La rete privata dell'infrastruttura {{site.data.keyword.Bluemix_notm}} viene offerta gratuitamente a utenti e dispositivi. Tutta la larghezza di banda sulla rete privata è illimitata e gratuita. La rete privata offre i seguenti vantaggi:
  * Replica degli ambienti dei dispositivi in altri data center per il failover
  * Accessibilità del sistema front-end ai server di database
  * Accesso e gestione sicuri ai tuoi sistemi

Per abilitare l'accesso utente alla rete privata, modifica l'accesso VPN nel portale clienti:
  1. Seleziona **Account** > **Accesso VPN** dalla barra dei menu.  
  2. Fai clic sul link nella colonna Accesso VPN.
  3. Seleziona un'opzione dal menu **Tipo di VPN** e fai clic su **Salva**.  

Per gli utenti negli account che utilizzano l'autenticazione con l'ID IBM, viene utilizzato il nome utente VPN SoftLayer per l'accesso VPN. Il nome utente VPN è definito nel profilo utente ed è diverso dal nome utente che, per impostazione predefinita, utilizza l'indirizzo e-mail e l'ID account dell'ID IBM.
{: tip}

Per ulteriori informazioni sull'utilizzo di una connessione VPN, vedi [Informazioni sulla VPN](/docs/infrastructure/iaas-vpn/about-vpn.html).

## Passo 4: sottoscrivi alle notifiche
{: #get-notified}

Per ricevere notifiche sui problemi di sistema che potrebbero verificarsi e sugli eventi di manutenzione pianificata, puoi sottoscrivere alle notifiche tramite l'Event Management System. Per impostazione predefinita, ti viene annullata la sottoscrizione alle notifiche quando crei un account o vieni aggiunto a un account.

Accedi a Event Management System nel portale clienti per specificare quali notifiche vuoi sottoscrivere:
  1. Seleziona **Account** > **Gestisci** > **Sottoscrizioni** dalla barra dei menu.
  2. Fai clic su una specifica sottoscrizione dall'elenco.
  3. Seleziona la casella di spunta **Sì** nella colonna Sottoscritto.
  4. Fai clic su **Visualizza tutte le sottoscrizioni** per tornare all'elenco di sottoscrizioni disponibili e sottoscrivere ad altri tipi secondo necessità.

## Passi successivi
{: #next-steps}

Dopo aver configurato il tuo account, vai al [catalogo {{site.data.keyword.Bluemix_notm}} ![Icona link esterno](../icons/launch-glyph.svg)](https://console.bluemix.net/catalog/?category=infrastructure){:new_window} e inizia a ordinare i dispositivi.
