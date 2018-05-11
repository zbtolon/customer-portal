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


# Single Sign-on konfigurieren
{: #customerportal_confssoserv}

Wenn Sie Masterbenutzer eines Kontos sind oder einen Verwaltungszugriff auf das Konto besitzen, können Sie das Single Sign-on konfigurieren. Die Konfiguration des Single Sign-on für die {{site.data.keyword.BluSoftlayer_full}}-Infrastruktur ist ein aus zwei Schritten bestehender Prozess.  Zuerst wählen Sie Ihren Identitätsprovider aus und konfigurieren ihn. Anschließend konfigurieren Sie die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für den Empfang der Authentifizierungsanforderung von Ihrem Identitätsprovider.
{:shortdesc}

## Identitätsprovider auswählen und konfigurieren
{: #cp_setupidprov}

Falls Sie noch keinen Identitätsprovider verwenden, wählen Sie zunächst einen Provider aus und konfigurieren Sie ihn. Bei {{site.data.keyword.BluSoftlayer_notm}} können Sie die folgenden Identitätsprovider verwenden:
* Ping Identity&reg;
* OneLogin&trade;
* IBM&reg; Cloud Security Enforcer
* IBM Cloud Identity Services
Weitere Informationen erhalten Sie bei Ihrem Vertriebsbeauftragten für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur.

Falls Sie bereits einen Identitätsprovider eingerichtet haben, können Sie bei Ihrem Identitätsprovider Unterstützung für bestimmte Schritte anfordern oder die folgenden allgemeinen Schritte zur Konfiguration des Identitätsproviders ausführen:
1. Bereiten Sie die Umgebung für Ihren Identitätsprovider vor, indem Sie die entsprechenden ausführbaren Dateien herunterladen und installieren.
2. Konfigurieren Sie Ihren Identitätsprovider für die Verwendung bei der {{site.data.keyword.BluSoftlayer_notm}}-Authentifizierung.

## {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für Single Sing-on konfigurieren
{: #cp_setupsso}

Sie müssen die folgenden erforderlichen Felder der Metadaten gemäß Security Assertion Markup Language&trade; (SAML&trade;) 2.0 aus Ihrem Identitätsprovider extrahieren, damit sie bei {{site.data.keyword.BluSoftlayer_notm}} verwendet werden können.
<dl>
<dt>Entitäts-ID</dt>
<dd>Die Entitäts-ID des Identitätsproviders.</dd>
<dt>URL für Single Sign-on</dt>
<dd>Der Endpunkt des Identitätsproviders für das Single Sign-on (SSO).</dd>
<dt>Zertifikat</dt>
<dd>Das Zertifikat des Identitätsproviders, mit dem Anforderungen signiert werden.</dd>
</dl>

Das folgende Feld ist optional:
<dl>
<dt>Zertifikatsfingerabdruck</dt>
<dd>Der Fingerabdruck des Zertifikats. Dieses Feld kann anstelle des vollständigen Zertifikats verwendet werden.</dd>
</dl>

Führen Sie die folgenden Schritte aus, um die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für den Empfang der Authentifizierungsanforderung von Ihrem Identitätsprovider zu konfigurieren:
1. Melden Sie sich bei Ihrem Identitätsprovider an, wenn Sie noch nicht angemeldet sind, und suchen Sie nach der Seite für die **SAML-Konfiguration**. Notieren Sie sich die folgenden Informationen:
  * Entitäts-ID
  * URL für Single Sign-on
  * Zertifikat (variiert je nach Identitätsprovider)
2. Melden Sie sich bei der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur als Masterbenutzer mit dem Namen und dem Kennwort des Masterbenutzers an, als der Sie Ihr SoftLayer-Konto erstellt haben.
3. Klicken Sie auf **Konto** > **Verwalten** > **SAML-Authentifizierung**.
4. Geben Sie die Metadaten für den **Identitätsprovider** ein.
5. Klicken Sie auf **Speichern**.
6. Klicken Sie auf **Konto** > **Verwalten** > **SAML-Authentifizierung**.
7. Klicken Sie auf **XML-Konfiguration herunterladen**, um die Metadaten für den Service-Provider herunterzuladen oder die Informationen zu notieren.
8. Verwenden Sie die Metadaten für den **Service-Provider**, um Ihren Identitätsprovider entsprechend den Anweisungen Ihres Identitätsproviders zu konfigurieren.  

Sie sollten jetzt in der Lage sein, sich unter Verwendung Ihrer eingebundenen ID bei der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur anzumelden. Weitere Informationen zu eingebundenen IDs finden Sie unter [{{site.data.keyword.Bluemix_notm}}-Anmeldung](/docs/account/adminpublic.html) und in der Veröffentlichung [IBMid Enterprise Federation Adoption Guide ![Symbol für externen Link](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}.
