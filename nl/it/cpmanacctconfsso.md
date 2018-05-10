---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-26"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Configurazione del single sign-on
{: #customerportal_confssoserv}

Se sei l'utente master di un account o hai accesso amministrativo ad esso, puoi configurare il single sign-on. La configurazione del single sign-on per l'infrastruttura {{site.data.keyword.BluSoftlayer_full}} è un processo in due fasi.  Innanzitutto, seleziona e configura il tuo provider di identità. Quindi, configura l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} per ricevere la richiesta di autenticazione dal provider di identità.
{:shortdesc}

## Selezione e configurazione del tuo provider di identità
{: #cp_setupidprov}

Se non disponi già di un provider di identità, devi selezionarne uno e configurarlo. Con {{site.data.keyword.BluSoftlayer_notm}} puoi utilizzare i seguenti provider di identità:
* Ping Identity&reg;,
* OneLogin&trade;,
* IBM&reg; Cloud Security Enforcer,
* IBM Cloud Identity Services.
Per ulteriori informazioni, contatta il rappresentante delle vendite della tua infrastruttura {{site.data.keyword.BluSoftlayer_notm}}.

Se non hai già configurato un provider di identità, per farlo puoi contattare il supporto del tuo provider per la procedura specifica o utilizzare la seguente procedura di livello superiore:
1. Prepara il tuo ambiente di provider di identità scaricando e installando il suo eseguibile.
2. Configura il tuo provider di identità in modo che funzioni con l'autenticazione {{site.data.keyword.BluSoftlayer_notm}}.

## Configurazione dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} per SSO
{: #cp_setupsso}

Dal tuo provider di identità, devi estrarre i seguenti campi obbligatori di informazioni sui metadati di Security Assertion Markup Language&trade; (SAML&trade;) 2.0 da utilizzare con {{site.data.keyword.BluSoftlayer_notm}}.
<dl>
<dt>ID entità</dt>
<dd>L'ID entità del provider di identità.</dd>
<dt>URL Single Sign-on</dt>
<dd>L'endpoint del provider di identità per SSO.</dd>
<dt>Certificato</dt>
<dd>Il certificato del provider di identità utilizzato per firmare le richieste.</dd>
</dl>

Il seguente campo è facoltativo:
<dl>
<dt>Impronta digitale certificato</dt>
<dd>L'impronta digitale del certificato. Questo campo può essere utilizzato al posto dell'intero certificato.</dd>
</dl>

Utilizza la seguente procedura per configurare l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} in modo da ricevere la richiesta di autenticazione dal tuo provider di identità:
1. Accedi al tuo provider di identità, se non sei già collegato, e individua la pagina **Configurazione SAML**. Nota le seguenti informazioni:
  * ID entità
  * URL Single sign-on
  * Certificato (questo varierà in base al tuo provider di identità.)
2. Accedi all'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} come utente master con il nome utente e la password master che hai utilizzato per creare il tuo account SoftLayer.
3. Fai clic su **Account** > **Gestisci** > **Autenticazione SAML**.
4. Immetti i metadati del **Provider di identità**.
5. Fai clic su **Salva**.
6. Fai clic su **Account** > **Gestisci** > **Autenticazione SAML**.
7. Fai clic su **Scarica configurazione XML** per scaricare i metadati del provider di servizio o annotare le informazioni.
8. Utilizza i metadati del **Provider di servizio** per configurare il tuo provider di identità in base alle istruzioni fornite da tale provider.  

Ora dovresti essere in grado di accedere all'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} utilizzando il tuo ID federato. Per ulteriori informazioni sugli ID federati, consulta [Registrazione per {{site.data.keyword.Bluemix_notm}}](/docs/account/adminpublic.html) e [IBMid Enterprise Federation Adoption Guide ![Icona link esterno](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}.
