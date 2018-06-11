---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-22"

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

In diesem Modell findet der folgende Prozess statt:
* Benutzer werden sowohl im Identitätsprovider als auch in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erstellt.
* Benutzerberechtigungen werden im Identitätsmanagementsystem (IMS) der {{site.data.keyword.BluSoftlayer}}-Infrastruktur mithilfe des Kundenportals oder der APIs für die {{site.data.keyword.BluSoftlayer}}-Infrastruktur zugeordnet.
* Benutzer authentifizieren sich beim Identitätsprovider und binden ihre Berechtigungsnachweise ein.
* Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur verarbeitet die Berechtigungsnachweise und die Zugriffssteuerung basiert auf den Berechtigungen, die für den Benutzer im IMS der {{site.data.keyword.BluSoftlayer}}-Infrastruktur definiert sind.

Konten für Benutzer, die auf die {{site.data.keyword.BluSoftlayer}}-Infrastruktur zugreifen müssen, werden in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur anfänglich mit automatisch generierten Kennwörtern erstellt. Alle Berechtigungen müssen in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur konfiguriert worden sein, bevor der Benutzer das Single Sign-on (SSO) über den Identitätsprovider verwenden kann. Gegenwärtig werden Berechtigungen für jeden Benutzer separat konfiguriert.

### Benutzer einrichten
Führen Sie zum Einrichten eines Benutzers die folgenden Schritte aus:

1. [Erstellen Sie Benutzer in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. Ordnen Sie Berechtigungen in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur zu.
3. Erstellen Sie Benutzer im Identitätsprovider.

Das Feld **E-Mail** oder **Benutzername** wird im Profil des einzelnen Benutzers für das Token von Security Assertion Markup Language&trade; (SAML&trade;) 2.0 verwendet. Dieses Token ordnet Benutzer zwischen dem Identitätsprovider und der {{site.data.keyword.BluSoftlayer}}-Infrastruktur zu.

### Beispielablauf für die Authentifizierung bei der Anmeldung
{: #exlogauthflowidprovicloud}

Der folgende Beispielablauf veranschaulicht, wie die Authentifizierung bei der Benutzeranmeldung funktionieren könnte, wenn Sie Benutzer im Identitätsprovider und in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erstellen:
1. Der Benutzer greift aus einer Browsersitzung heraus auf die URL des Identitätsproviders zu.
2. Der Identitätsprovider authentifiziert den Benutzer, beispielsweise über LDAP.
3. Der Identitätsprovider gibt Antworten in SAML 2.0 zurück.
4. Der Identitätsprovider sendet eine Antwort in SAML 2.0 an den Service-Provider, in diesem Fall die {{site.data.keyword.BluSoftlayer}}-Infrastruktur, um die Benutzer-ID zu authentifizieren.
5. Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur validiert die Antwort in SAML 2.0.
6. Der Benutzer wird beim Kundenportal der {{site.data.keyword.BluSoftlayer}}-Infrastruktur auf Grundlage der als vertrauenswürdig anerkannten Konfiguration zwischen dem Identitätsprovider und der {{site.data.keyword.BluSoftlayer}}-Infrastruktur angemeldet.


## Benutzer im Identitätsprovider erstellen
{: #cp_scenario2idp}

Bei diesem Modell findet Folgendes statt:
* Im Identitätsprovider werden Rollen erstellt und dem Benutzer zugeordnet.
* Im IMS der {{site.data.keyword.BluSoftlayer}}-Infrastruktur werden mithilfe der APIs für die {{site.data.keyword.BluSoftlayer}}-Infrastruktur Rollen- und Berechtigungszuordnungen konfiguriert.
* Benutzer authentifizieren sich beim Identitätsprovider und binden ihre Berechtigungsnachweis und Rollenattribute ein.
* Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur überprüft die Benutzerberechtigungsnachweise und die Rollenattribute. Wenn die Rollen, die den Benutzern von ihrem Identitätsprovider zugewiesen sind, mit den Rollen in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur übereinstimmen, erhalten diese Benutzer Berechtigungen für diese Rollen, wenn sie sich bei der {{site.data.keyword.BluSoftlayer}}-Infrastruktur anmelden.
* Die vom Identitätsprovider erstellten Benutzer gelten als eingebunden (föderiert), da die Authentifizierung für sie und ihre Rollen über SAML 2.0 erfolgt.

### Rolle für einen Benutzer konfigurieren
{: #cp_set-up-user-role}

Führen Sie die folgenden Schritte aus, um eine Rolle für einen Benutzer zu konfigurieren:

1. Richten Sie Rollen mithilfe der APIs für die {{site.data.keyword.BluSoftlayer}}-Infrastruktur ein.
2. Richten Sie Rollen im Identitätsprovider ein.
3. Stellen Sie sicher, dass die in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur und im Identitätsprovider definierten Rollen identische Namen besitzen.

### Benutzer einrichten
{: #setupuser}

Führen Sie zum Einrichten eines Benutzers die folgenden Schritte aus:

1. Richten Sie Benutzer im Identitätsprovider ein.
2. Ordnen Sie Rollen im Identitätsprovider zu Benutzern zu.

In diesem Szenario müssen Sie keine Benutzer manuell in der {{site.data.keyword.BluSoftlayer}}-Infrastruktur erstellen.

### Beispielablauf für die Authentifizierung bei der Benutzeranmeldung
{: #exlogauthflowidprov}

Der folgende Beispielablauf veranschaulicht, wie die Authentifizierung bei der Benutzeranmeldung funktionieren könnte, wenn Sie Benutzer im Identitätsprovider erstellen:
1. Der Benutzer greift aus einer Browsersitzung heraus auf die URL des Identitätsproviders zu.
2. Der Identitätsprovider authentifiziert den Benutzer, beispielsweise über LDAP.
3. Der Identitätsprovider gibt Antworten in SAML 2.0 zurück.
4. Der Identitätsprovider sendet eine Antwort in SAML 2.0 an den Service-Provider, in diesem Fall die {{site.data.keyword.BluSoftlayer}}-Infrastruktur, um die Benutzerrolle zu authentifizieren.
5. Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur validiert die Antwort in SAML 2.0.
6. Die {{site.data.keyword.BluSoftlayer}}-Infrastruktur leitet den Benutzer an das Kundenportal weiter.
7. Der Benutzer wird beim Kundenportal der {{site.data.keyword.BluSoftlayer}}-Infrastruktur angemeldet.

Informieren Sie sich über die Prozeduren Ihres Identitätsproviders für die Einrichtung neuer Rollen und deren Zuordnung zur {{site.data.keyword.BluSoftlayer}}-Infrastruktur.
