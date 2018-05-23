---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-10"

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:tip: .tip}
{:codeblock: .codeblock}
{:pre: .pre}
{:new_window: target="_blank"}

# Utilizzo di account ID IBM con l'infrastruttura {{site.data.keyword.BluSoftlayer_notm}}
{: #customerportal_ibmid}

L'autenticazione nell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} adesso utilizza l'ID IBM per fornire un singolo accesso in {{site.data.keyword.Bluemix_notm}}.
{:shortdesc}

Se disponi di un account SoftLayer esistente, puoi passare a un ID IBM. Una procedura guidata di migrazione può aiutarti in questo passaggio. Per ulteriori informazioni, vedi [Passaggio all'ID IBM](/docs/account/softlayerlink.html#switching-to-ibmid).

## Associazione di più account SoftLayer a un ID IBM
{: #cp_mapmultclinfrto1ibmid}

Puoi associare un ID IBM a più account SoftLayer utilizzando un'e-mail ID IBM esistente durante l'impostazione dell'account. Al singolo ID IBM è possibile associare un solo utente dell'infrastruttura {{site.data.keyword.BluSoftlayer_notm}} per ogni account. L'ID IBM deve essere univoco all'interno di ogni account SoftLayer. Tuttavia, un utente con accesso a più account SoftLayer può utilizzare un ID IBM per accedere a diversi account SoftLayer.

Ad esempio, un ID IBM può essere associato all'utente master negli account A e B e a un ulteriore utente negli account C e D. Uno degli account associato a tale ID IBM è l'account predefinito. Di solito, l'account predefinito è quello che è stato associato per primo all'ID IBM. Tuttavia, puoi cambiare l'account predefinito utilizzando una funzione di passaggio tra account nel portale clienti.

![Più account SoftLayer a un ID IBM](images/ibmid-image.png)

Per un utente che dispone dell'accesso ID IBM a più account e per cui è abilitata l'autenticazione a due fattori, è richiesto un codice di verifica appropriato per tale autenticazione durante l'accesso e il passaggio tra gli account.
