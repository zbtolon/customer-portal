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

# Identitätseinbindung festlegen
{: #cp_setupidfed}

Durch das Festlegen der Identitätseinbindung können Sie einem Service-Provider wie beispielsweise {{site.data.keyword.BluSoftlayer_full}} Infrastructure Management System (IMS) die Verarbeitung von Sicherheitstoken ermöglichen, die zu Authentifizierungs- und Autorisierungszwecken durch ein anerkanntes Identitätssystem generiert werden.
{:shortdesc}

Zum Festlegen der Identitätseinbindung in das Single Sign-on der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur können Sie eines der folgenden Verfahren verwenden:
* Benutzer im Identitätsprovider und in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erstellen
* Benutzer im Identitätsprovider erstellen

Eine Rolle definiert für den Service-Provider, für welche Aktionen der Benutzer (mittels Berechtigungen) im System autorisiert ist, nachdem er authentifiziert wurde. Beispielsweise kann die Rolle *Benutzer* nur zum Aufrufen verschiedener Anzeigen, jedoch nicht zum Aktualisieren oder Hinzufügen berechtigt sein.

Einer einzigen Rolle können mehrere Benutzer zugeordnet sein. Wenn eine Rolle im Identitätsprovider, nicht jedoch in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur besteht, kann sich der Benutzer außerdem weiterhin bei der {{site.data.keyword.BluSoftlayer}}-Infrastruktur anmelden, besitzt jedoch keine Berechtigungen, die einer Rolle zugeordnet sind.
{: tip}


## Benutzer im Identitätsprovider und in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erstellen
{: #cp_scenario1both}

Bei diesem Modell findet Folgendes statt:
* Benutzer werden sowohl im Identitätsprovider als auch in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erstellt.
* Benutzerberechtigungen werden im Identitätsmanagementsystem (IMS) der {{site.data.keyword.BluSoftlayer}}-Infrastruktur mithilfe des Kundenportals oder der APIs für die {{site.data.keyword.BluSoftlayer}}-Infrastruktur zugeordnet.
* Benutzer authentifizieren sich beim Identitätsprovider und binden ihre Berechtigungsnachweise ein.
* Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur verarbeitet die Berechtigungsnachweise; die Zugriffssteuerung basiert auf den Berechtigungen, die für den Benutzer im IMS der {{site.data.keyword.BluSoftlayer}}-Infrastruktur definiert sind.

Konten für Benutzer, die auf die {{site.data.keyword.BluSoftlayer}}-Infrastruktur zugreifen müssen, werden in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur anfänglich mit automatisch generierten Kennwörtern erstellt. Alle Berechtigungen müssen in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur konfiguriert worden sein, bevor der Benutzer das Single Sign-on (SSO) über den Identitätsprovider verwenden kann. Gegenwärtig werden Berechtigungen für jeden Benutzer separat konfiguriert.

### Benutzer einrichten
Führen Sie zum Einrichten eines Benutzers die folgenden Schritte aus:

1. [Erstellen Sie Benutzer in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. Ordnen Sie Berechtigungen in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur zu.
3. Erstellen Sie Benutzer im Identitätsprovider.

Das Feld **E-Mail** oder **Benutzername** wird im Profil des individuellen Benutzers für das Token von Security Assertion Markup Language&trade; (SAML&trade;) 2.0 verwendet, das Benutzer zwischen dem Identitätsprovider und der {{site.data.keyword.BluSoftlayer}}-Infrastruktur zuordnet.

### Beispielablauf für die Authentifizierung bei der Anmeldung
Der folgende Beispielablauf veranschaulicht, wie die Authentifizierung bei der Benutzeranmeldung funktionieren könnte, wenn Sie Benutzer im Identitätsprovider und in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erstellen:
1. Der Benutzer greift aus einer Browsersitzung heraus auf die URL des Identitätsproviders zu.
2. Der Identitätsprovider authentifiziert den Benutzer, beispielsweise über LDAP.
3. Der Identitätsprovider gibt Antworten in SAML 2.0 zurück.
4. Der Identitätsprovider sendet eine Antwort in SAML 2.0 an den Service-Provider, in diesem Fall die {{site.data.keyword.BluSoftlayer}}-Infrastruktur, um die Benutzer-ID zu authentifizieren.
5. Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur validiert die Antwort in SAML 2.0.
6. Der Benutzer wird beim Kundenportal der {{site.data.keyword.BluSoftlayer}}-Infrastruktur auf Grundlage der anerkannten Konfiguration zwischen dem Identitätsprovider und der {{site.data.keyword.BluSoftlayer}}-Infrastruktur angemeldet.


## Benutzer im Identitätsprovider erstellen
{: #cp_scenario2idp}

Bei diesem Modell findet Folgendes statt:
* Im Identitätsprovider werden Rollen erstellt und dem Benutzer zugeordnet.
* Im IMS der {{site.data.keyword.BluSoftlayer}}-Infrastruktur werden mithilfe der APIs für die {{site.data.keyword.BluSoftlayer}}-Infrastruktur Rollen- und Berechtigungszuordnungen konfiguriert.
* Benutzer authentifizieren sich beim Identitätsprovider und binden ihre Berechtigungsnachweis und Rollenattribute ein.
* Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur verarbeitet die Benutzerberechtigungsnachweise und die Rollenattribute. Falls die vom Identitätsprovider des Benutzers zugeordnete Rolle mit einer Rolle in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur übereinstimmt, werden dem Benutzer die Berechtigungen für diese Rolle erteilt, wenn er sich bei der {{site.data.keyword.BluSoftlayer}}-Infrastruktur anmeldet.
* Im Identitätsprovider erstellte Benutzer werden als eingebunden betrachtet, weil sie und ihre Rollen über SAML 2.0 authentifiziert werden.

### Rolle für einen Benutzer konfigurieren
Führen Sie die folgenden Schritte aus, um eine Rolle für einen Benutzer zu konfigurieren:

1. Richten Sie Rollen mithilfe der APIs für die {{site.data.keyword.BluSoftlayer}}-Infrastruktur ein.
2. Richten Sie Rollen im Identitätsprovider ein.
3. Stellen Sie sicher, dass die in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur und im Identitätsprovider definierten Rollen identische Namen besitzen.

### Benutzer einrichten
{: #setupuser}

Führen Sie zum Einrichten eines Benutzers die folgenden Schritte aus:

1. Richten Sie Benutzer im Identitätsprovider ein.
2. Ordnen Sie Rollen im Identitätsprovider zu Benutzern zu.

In diesem Szenario ist es nicht erforderlich, dass Sie in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur Benutzer manuell erstellen.

### Beispielablauf für die Authentifizierung bei der Benutzeranmeldung
Der folgende Beispielablauf veranschaulicht, wie die Authentifizierung bei der Benutzeranmeldung funktionieren könnte, wenn Sie Benutzer im Identitätsprovider erstellen:
1. Der Benutzer greift aus einer Browsersitzung heraus auf die URL des Identitätsproviders zu.
2. Der Identitätsprovider authentifiziert den Benutzer, beispielsweise über LDAP.
3. Der Identitätsprovider gibt Antworten in SAML 2.0 zurück.
4. Der Identitätsprovider sendet eine Antwort in SAML 2.0 an den Service-Provider, in diesem Fall die {{site.data.keyword.BluSoftlayer}}-Infrastruktur, um die Benutzerrolle zu authentifizieren.
5. Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur validiert die Antwort in SAML 2.0.
6. Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur leitet den Benutzer an das Kundenportal weiter.
7. Der Benutzer wird beim Kundenportal der {{site.data.keyword.BluSoftlayer}}-Infrastruktur angemeldet.

Informieren Sie sich über die Prozeduren Ihres Identitätsproviders für die Einrichtung neuer Rollen und deren Zuordnung zur {{site.data.keyword.BluSoftlayer}}-Infrastruktur.
