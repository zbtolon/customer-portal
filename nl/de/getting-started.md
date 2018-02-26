---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Lernprogramm 'Einführung'
{: #getting-started}

In diesem Lernprogramm werden Sie durch den Prozess geführt, mit dem Sie Ihr SoftLayer-Konto betriebsbereit machen, damit Sie anschließend Ihre Infrastrukturressourcen bestellen und verwalten können.
{:shortdesc}

## Vorbereitende Schritte
{: #prereqs}

Sie benötigen ein [{{site.data.keyword.Bluemix}}-Konto ![Symbol für externen Link](../icons/launch-glyph.svg "Symbol für externen Link")](https://control.bluemix.net/){:new_window}. Melden Sie sich mit den Berechtigungsnachweisen Ihrer IBMid beim Kundenportal an. Die meisten Benutzer verwenden die [IBMid](/docs/account/softlayerlink.html#switchtoIBMid) für die Authentifizierung.

Wenn Sie zum Anmelden an Ihrem Konto nicht die IBMid zur Authentifizierung verwenden, melden Sie sich beim Kundenportal mit Ihren eindeutigen Berechtigungsnachweisen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur an.
{: tip}

## Schritt 1: Konto einrichten
{: #account-setup}

Zur Einrichtung Ihres Kontos müssen Sie die Kontaktinformationen und Abrechnungsdetails für das Konto prüfen:
 * Um die Details für den Ansprechpartner im Unternehmen zu prüfen, navigieren Sie zu **Konto** > **Verwalten** > **Ansprechpartner im Unternehmen**. Die Informationen zum Ansprechpartner im Unternehmen für Ihr Konto werden verwendet, um Sie über Probleme mit oder Änderungen an Ihrem Konto zu benachrichtigen.
 * Um die Details für das Unternehmensprofil zu prüfen, navigieren Sie zu **Konto** > **Verwalten** > **Unternehmensprofil**. Die Informationen zum Unternehmensprofil enthalten Details über den primären Kontoeigner.
 * Um die Details für die Abrechnung zu prüfen, navigieren Sie zu **Konto** > **Abrechnung** > **Zahlungsmethode**. Die monatliche Zahlungsmethode ist die Kreditkarte, die regelmäßig mit Zahlungen für Ihr Konto belastet wird.

## Schritt 2: Benutzer hinzufügen und Berechtigungen zuordnen
{: #users-permissions}

Um Benutzer zu Ihrem Konto hinzuzufügen und deren Anfangsberechtigungen festzulegen, navigieren Sie zu **Konto** > **Benutzer**.
 * Um Benutzer für sowohl Plattform- als auch Infrastrukturressourcen in Ihrem Konto auf Grundlage der jeweils von Ihnen zugeordneten Berechtigungen einzuladen, klicken Sie auf **Benutzer einladen**. Anschließend werden Sie zur Benutzerschnittstelle von {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) geleitet, in der Sie Benutzer einladen und den Zugriff zuordnen können. Weitere Informationen finden Sie unter [Benutzer einladen und Zugriff zuordnen](/docs/iam/iamuserinv.html).
 * Um Benutzer nur mit VPN-Zugriff hinzuzufügen, klicken Sie auf **Reine VPN-Benutzer hinzufügen**. Geben Sie die persönlichen Informationen ein, definieren Sie die Portalberechtigungen und legen Sie den Gerätezugriff für den Benutzer fest.

Wenn Sie in der erstmaligen Einladung Infrastrukturberechtigungen festlegen, wählen Sie eines der drei Berechtigungssets 'Nur anzeigen', 'Basisbenutzer' oder 'Superuser' aus. Nachdem Benutzer die Einladung angenommen haben, können Sie deren Zugriff anpassen, indem Sie die Portalberechtigungen bearbeiten. Weitere Informationen finden Sie unter [Infrastrukturberechtigungen](/docs/iam/infrastructureaccess.html).
{: tip}

## Schritt 3: Zugriff auf das private Netz der {{site.data.keyword.Bluemix_notm}}-Infrastruktur ermöglichen
{: #enable-private-network}

Das private Netz der {{site.data.keyword.Bluemix_notm}}-Infrastruktur wird kostenlos für Benutzer und Geräte angeboten. Die gesamte für das private Netz genutzte Bandbreite wird nicht gemessen und ist als Ergänzung zu verstehen. Das private Netz bietet viele Vorzüge, unter anderem die Replizierung von Geräteumgebungen in anderen Rechenzentren für das Failover, die Zugriffsmöglichkeit auf Datenbankserver von Front-End-Systemen sowie den sicheren Zugriff und die sichere Verwaltung für Ihre Systeme.

Um Benutzern den Zugriff auf das private Netz zu ermöglichen, bearbeiten Sie den VPN-Zugriff im Kundenportal:
  1. Wählen Sie in der Menüleiste die Optionen **Konto** > **VPN-Zugriff** aus.  
  2. Klicken Sie in der Spalte 'VPN-Zugriff' auf den Link.
  3. Wählen Sie eine Option im Menü **VPN-Typ** aus und klicken Sie auf **Speichern**.  

Für Benutzer in Konten, die die IBMid-Authentifizierung verwenden, wird der SoftLayer-VPN-Benutzername für den VPN-Zugriff verwendet. Der VPN-Benutzername ist im Benutzerprofil definiert. Der VPN-Benutzername ist nicht mit dem Benutzernamen identisch, der standardmäßig aus der IBMid-E-Mail-Adresse und der Konto-ID besteht.
{: tip}

## Schritt 4: Benachrichtigungen abonnieren
{: #get-notified}

Damit Sie über möglicherweise auftretende Systemprobleme und planmäßige Wartungsereignisse informiert werden, können Sie über das Ereignismanagementsystem (Event Management System, EMS) Benachrichtigungen abonnieren. Wenn Sie ein Konto erstellen oder zu einem Konto hinzugefügt werden, besteht standardmäßig kein Abonnement von Benachrichtigungen.

Greifen Sie auf das Ereignismanagementsystem im Kundenportal zu, um die Benachrichtigungen auszuwählen, die Sie abonnieren wollen:
  1. Wählen Sie in der Menüleiste die Optionen **Konto** > **Verwalten** > **Abonnements** aus.
  2. Klicken Sie in der angezeigten Liste auf ein bestimmtes Abonnement.
  3. Wählen Sie in der Spalte 'Abonniert' das Kontrollkästchen **Ja** aus.
  4. Klicken Sie auf **Alle Abonnements anzeigen**, um zur Liste der verfügbaren Abonnements zurückzukehren und bei Bedarf weitere Typen zu abonnieren.

## Nächste Schritte
{: #next-steps}

Nachdem Sie Ihr Konto eingerichtet haben, können Sie den [{{site.data.keyword.Bluemix_notm}}-Katalog ![Symbol für externen Link](../icons/launch-glyph.svg)](https://console.bluemix.net/catalog/?category=infrastructure){:new_window} aufrufen und mit dem Bestellen von Geräten beginnen.
