---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-12"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Bare-Metal-Server einrichten
{: #customerportal_setupbaremetal}

Sie können einen Bare-Metal-Server als dedizierten Server einrichten.
{:shortdesc}

Führen Sie die folgenden Schritte aus, um einen Bare-Metal-Server einzurichten:

1. Melden Sie sich beim {{site.data.keyword.BluSoftlayer_full}}-Kundenportal mit Ihren eindeutigen Berechtigungsnachweisen an.

2. Klicken Sie im Menü auf **Geräte** > **Geräteliste** und suchen Sie Ihr System. In der Geräteliste sind alle Ihre Geräte detailliert ausgeführt. Dort können Sie Geräte verwalten, Upgrades für Geräte durchführen oder Bandbreitennutzungsdiagramme erstellen.

3. Wählen Sie für die Verwaltung Ihres Servers eine der folgenden Arten aus:
  * Klicken Sie auf den Pfeil neben dem Gerätenamen, um eine Zusammenfassung anzuzeigen und Ihre Geräte über die Snapshotansicht zu verwalten.
  * Klicken Sie auf den Gerätenamen des Servers, um eine detaillierte Liste anzuzeigen und Ihre Geräte über die Anzeige 'Gerätedetails' zu verwalten.

4. Dokumentieren Sie die IP-Adresse und die Berechtigungsnachweise für den Server an einer sicheren Position, damit Sie bei Bedarf rasch auf die Details zugreifen können, ohne sich dafür jedes Mal beim Kundenportal anmelden zu müssen. Sie können diese Details sowohl für ein einzelnes Gerät als auch für alle zu Ihrem Konto zugehörigen Geräte dokumentieren.
  * Zeigen Sie einzelne Geräte-IPs von der Geräteliste an.
  * Zeigen Sie einzelne Geräterootkennwörter in der Snapshotansicht für das Gerät an.
  * Zeigen Sie mehrere Geräte-IPs mithilfe der Option zum Herunterladen von CSV**** für die **Geräteliste** an. Wählen Sie anschließend die Option zum Herunterladen von CSV**** im Katalog **Einstellungen** aus, um eine vollständige Liste von Geräten und Details in Tabellenformat herunterzuladen.

5. Aktualisieren Sie die Berechtigungsnachweise für Betriebssysteme und andere Software. Allen Softwareprodukten, die während des Bereitstellungsprozesses auf Ihr Gerät geladen wurden, wurden temporäre Berechtigungsnachweise zugeordnet. Sie können diese Berechtigungsnachweise auf der Registerkarte 'Kennwörter' jedes Geräts im Kundenportal anzeigen und verwalten. Verwenden Sie diese temporären Berechtigungsnachweise beim erstmaligen Zugriff auf Ihre Software und ändern Sie dann das Kennwort zu Ihrer Software unter Verwendung eines sicheren Kennworts, das aus einer Kombination aus Buchstaben, Zahlen und Symbolen besteht. Optional können Sie Kennwortaktualisierungen auf der Registerkarte 'Kennwörter' der einzelnen Geräte speichern. Wenn Sie Kennwörter im Kundenportal speichern, kann jedoch jede Person, die über Zugriff auf das Konto und entsprechende Berechtigungen verfügt, die in der Anzeige für Kennwörter gespeicherten Kennwörter anzeigen.

6. Greifen Sie auf Ihren Server auf dem privaten Netz zu. Sie können das private Netz der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur verwenden, um mit Ihren Geräten über Remote Desktop (RDP) mit SSH und KVM über IP zu interagieren. Sie können das Tool 'VPN-Zugriff' für die private Netzverbindung zum nächsten SSL-VPN-Endpunkt oder zum Endpunkt Ihrer Wahl verwenden. VPN-Zugriff ist auch für die Interaktion mit verschiedenen Services erforderlich. Um auf das private Netz zuzugreifen, bearbeiten Sie den VPN-Zugriff des Benutzers über die Benutzerliste. Klicken Sie für den Zugriff auf die Benutzerliste auf **Konto** > **Benutzer** > **Benutzerliste**. Verwenden Sie die Seite [Virtuelles privates Netz ![Symbol für externen Link](../icons/launch-glyph.svg)](https://www.softlayer.com/VPN-Access){:new_window}, um eine Verbindung zu einer der verschiedenen VPN-Optionen herzustellen.

7. Richten Sie die Überwachung ein, um den Status Ihres Servers überprüfen zu können und Informationen zur Notwendigkeit einer Skalierung abrufen zu können. Sie können Standardüberwachungsservices oder Nimsoft-Überwachungsservices verwenden. Sie können bei der Methode 'ping-and-respond' die Standardüberwachung (oder Basisüberwachung) verwenden, indem Sie entweder einen langsamen Ping oder einen Serviceping aus dem Kundenportal verwenden. Ferner können Sie auch die Nimsoft-Überwachung oder die erweiterte Überwachung aus dem Kundenportal oder in einer von drei möglichen Stufen verwenden: Basis, Erweitert und Premium.

8. Schützen Sie Ihr System. Verwenden Sie die verfügbaren Hardware-Firewalls um sicherzustellen, dass Ihr Gerät jederzeit sicher ist. Sie können Hardware-Firewalls bedarfsgerecht ohne Ausfallzeit bereitstellen, wenn die Regeln ordnungsgemäß festgelegt wurden, um Ihren Server vor unerwünschter Aktivität zu schützen. Nach dem Anfordern Ihrer Firewall muss sie aktiviert werden und es müssen Regeln festgelegt werden.

9. Planen Sie Sicherungen um sicherzustellen, dass Ihre Daten sicher außerhalb Ihres Geräts gespeichert werden und um sie bei Verlust erneut laden zu können. Sie können aus einer Vielfalt von Backup-Services auswählen, um Ihre Daten an einer sicheren Position zu speichern:
  * EVault Backup ist ein automatisiertes, agentenbasiertes Sicherungssystem. Dies ist eine gängige, komfortable und wartungsfreie Lösung zur Verwaltung Ihres Geräts. Sie ist kompatibel mit Microsoft-Software, einschließlich Exchange und SQL (über zusätzliche Plug-ins). EVault-Benutzer interagieren mit diesem Service über die webbasierte EVault-Anwendung WebCC.
  * R1Soft Continuous Data Protection (CDP) kann auf Ihrem Server oder auf der selbstverwalteten virtuellen Maschine installiert werden. Diese Lösung empfiehlt sich, wenn Sie nach einer einzigen Schnittstelle zum Verwalten all Ihrer Sicherungen suchen. Sie interagieren mit R1Soft CDP über Ihr proprietäres Managementsystem, das die Installation von Agenten auf virtuellen Maschinen ermöglicht und Datenbank-Plug-ins für zusätzliche Funktionalität bietet.
