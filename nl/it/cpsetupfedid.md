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

# Configurazione della federazione dell'identità
{: #cp_setupidfed}

Puoi configurare la federazione dell'identità per consentire a un provider di servizi, ad esempio {{site.data.keyword.BluSoftlayer_full}} Infrastructure Management System (IMS), di utilizzare i token di sicurezza generati da un sistema di identità attendibile per scopi di autenticazione e autorizzazione.
{:shortdesc}

Puoi configurare la federazione dell'identità nel SSO dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} utilizzando uno dei seguenti modi:
* Creazione di utenti nel provider di identità e nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}
* Creazione di utenti nel provider di identità

Un ruolo definisce, per il provider di servizi, ciò che l'utente è autorizzato a fare (attraverso le autorizzazioni) nel proprio sistema dopo che l'utente è stato autenticato. Ad esempio, il ruolo *Utente* potrebbe essere autorizzato solo a visualizzare le diverse schermate, ma non a effettuare aggiornamenti o aggiunte.

Più utenti possono essere assegnati a un singolo ruolo. Inoltre, se un ruolo esiste nel provider di identità ma non nell'infrastruttura {{site.data.keyword.BluSoftlayer}}, l'utente può comunque accedere all'infrastruttura {{site.data.keyword.BluSoftlayer}} ma non ha alcuna autorizzazione assegnata a un ruolo.
{: tip}


## Creazione di utenti nel provider di identità e nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}
{: #cp_scenario1both}

In questo modello, si verifica quanto segue:
* Gli utenti vengono creati nel provider di identità e nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.
* Le autorizzazioni utente vengono assegnate nell'IMS dell'infrastruttura {{site.data.keyword.BluSoftlayer}} utilizzando il portale del cliente o le API dell'infrastruttura {{site.data.keyword.BluSoftlayer}}.
* Gli utenti si autenticano con il provider di identità e federano le proprie credenziali.
* L'infrastruttura {{site.data.keyword.BluSoftlayer}} utilizza le credenziali e il controllo dell'accesso si basa sulle autorizzazioni definite per l'utente nell'IMS dell'infrastruttura {{site.data.keyword.BluSoftlayer}}.

Gli account per gli utenti che necessitano dell'accesso all'infrastruttura {{site.data.keyword.BluSoftlayer}} vengono inizialmente creati nell'infrastruttura {{site.data.keyword.BluSoftlayer}} con password casuali. Tutte le autorizzazioni devono essere configurate nell'infrastruttura {{site.data.keyword.BluSoftlayer}} prima che l'utente possa utilizzare SSO tramite il provider di identità. Attualmente, le autorizzazioni sono configurate in base al singolo utente.

### Configurazione di un utente
Utilizza la seguente procedura per configurare un utente:

1. [Crea gli utenti nell'infrastruttura {{site.data.keyword.BluSoftlayer}}](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. Assegna le autorizzazioni nell'infrastruttura {{site.data.keyword.BluSoftlayer}}.
3. Crea gli utenti nel provider di identità.

Il campo **E-mail** o **Nome utente** all'interno del profilo del singolo utente è utilizzato per il token SAML&trade; (Security Assertion Markup Language&trade;) 2.0, che associa gli utenti tra il provider di identità e l'infrastruttura {{site.data.keyword.BluSoftlayer}}.

### Flusso di esempio per l'autenticazione di accesso
Di seguito è riportato un flusso di esempio di come potrebbe funzionare l'autenticazione di accesso utente quando crei gli utenti nel provider di identità e nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}:
1. L'utente accede all'URL del provider di identità da una sessione del browser.
2. Il provider di identità autentica l'utente, ad esempio tramite il suo LDAP.
3. Il provider di identità restituisce risposte SAML 2.0.
4. Il provider di identità invia una risposta SAML 2.0 al provider di servizio, in questo caso all'infrastruttura {{site.data.keyword.BluSoftlayer}}, per autenticare l'ID utente.
5. L'infrastruttura {{site.data.keyword.BluSoftlayer}} convalida la risposta SAML 2.0.
6. L'utente ha effettuato l'accesso al portale del cliente dell'infrastruttura {{site.data.keyword.BluSoftlayer}} in base alla configurazione affidabile tra il provider di indentità e l'infrastruttura {{site.data.keyword.BluSoftlayer}}.


## Creazione di utenti nel provider di identità
{: #cp_scenario2idp}

In questo modello, accadono le seguenti cose:
* Vengono creati i ruoli nel provider di identità e quindi assegnati all'utente.
* Le assegnazioni di ruoli e autorizzazioni sono configurate nell'IMS dell'infrastruttura {{site.data.keyword.BluSoftlayer}} utilizzando le API dell'infrastruttura {{site.data.keyword.BluSoftlayer}}. 
* Gli utenti si autenticano con il provider di identità e federano le proprie credenzial e gli attributi del ruolo. 
* L'infrastruttura {{site.data.keyword.BluSoftlayer}} utilizza le credenziali dell'utente e gli attributi del ruolo. Se il ruolo assegnato dal provider di identità dell'utente corrisponde a un ruolo nell'infrastruttura {{site.data.keyword.BluSoftlayer}}, all'utente vengono concesse le autorizzazioni per tale ruolo durante l'accesso all'infrastruttura {{site.data.keyword.BluSoftlayer}}.
* Gli utenti creati nel provider di identità sono considerati federati in quanto essi e i relativi ruoli sono autenticati tramite SAML 2.0.

### Configurazione di un ruolo per un utente
Utilizza la seguente procedura per configurare un ruolo per un utente:

1. Configura i ruoli tramite l'API dell'infrastruttura {{site.data.keyword.BluSoftlayer}}.
2. Configura i ruoli nel provider di identità..
3. Assicurati che i ruoli definiti nell'infrastrutttura {{site.data.keyword.BluSoftlayer}} e nel provider di identità abbiano lo stesso nome.

### Configurazione di un utente
{: #setupuser}

Utilizza la seguente procedura per configurare un utente:

1. Configura gli utenti nel provider di identità.
2. Assegna ruoli agli utenti nel provider di identità.

In questo scenario, non è necessario creare manualmente gli utenti nell'infrastruttura {{site.data.keyword.BluSoftlayer}}.

### Flusso di esempio per l'autenticazione di accesso utente
Di seguito è riportato un flusso di esempio di come potrebbe funzionare l'autenticazione di accesso utente quando crei gli utenti nel provider di identità:
1. L'utente accede all'URL del provider di identità da una sessione del browser.
2. Il provider di identità autentica l'utente, ad esempio tramite il suo LDAP.
3. Il provider di identità restituisce risposte SAML 2.0.
4. Il provider di identità invia una risposta SAML 2.0 al provider di servizio, in questo caso all'infrastruttura {{site.data.keyword.BluSoftlayer}}, per autenticare il ruolo utente.
5. L'infrastruttura {{site.data.keyword.BluSoftlayer}} convalida la risposta SAML 2.0.
6. L'infrastruttura {{site.data.keyword.BluSoftlayer}} reindirizza l'utente al portale del cliente.
7. L'utente ha effettuato l'accesso al portale del cliente dell'infrastruttura {{site.data.keyword.BluSoftlayer}}.

Esamina le procedure del tuo provider di identità per informazioni sulla configurazione di nuovi ruoli e su come associarli all'infrastruttura {{site.data.keyword.BluSoftlayer}}.
