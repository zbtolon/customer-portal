---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-16"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Systeme schützen
{: #customerportal_protsys}

Durch den Schutz Ihrer Systeme können Sie dafür sorgen, dass die Systeme reibungslos und ohne unnötige Unterbrechungen ausgeführt werden.

## Privates Netz verwenden
{: #cp_bpuseprivnet}

Durch Verwendung des privaten Netzes der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur können Sie Ihre Geräte in einer Umgebung mit der größtmöglichen Sicherheit verwalten. Hier interagieren Sie nach Möglichkeit über eine VPN-Verbindung mit Ihren Geräten und ermöglichen eine netzübergreifende Verarbeitung, damit Ihre Systeme über das private Netz miteinander kommunizieren. Um auf das private Netz zuzugreifen, bearbeiten Sie den VPN-Zugriff des Benutzers über die [Benutzerliste ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Verwenden Sie die Liste [Virtuelles privates Netz ![Symbol für externen Link](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window}, um eine Verbindung zu einer der verschiedenen VPN-Optionen herzustellen.

### RDP, SSH oder Steuerports nicht im öffentlichen Netz belassen
{: #cp_bpnordpsshcponpubnet}

Das öffentliche Netz ist für viele Zwecke hervorragend geeignet. Es gibt jedoch bestimmte Aspekte, die dazu führen können, dass Ihr System anfällig bleibt, wenn sie über geöffnete Ports im öffentlichen Netz verfügbar bleiben. Schützen Sie sich selbst, indem Sie RDP inaktivieren oder SSH im öffentlichen Netz beschränken. Falls diese Services im öffentlichen Netz verfügbar sein müssen, kann es sinnvoll sein, RDP oder SSH an eine benutzerdefinierte Portnummer zu versetzen.

## Daten durch regelmäßige Sicherungen schützen
{: #cp_bpsafedataregback}

Planen Sie Sicherungen um sicherzustellen, dass Ihre Daten sicher außerhalb Ihres Geräts gespeichert werden und um sie bei Verlust erneut laden zu können.

Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur bietet mehrere Sicherungslösungen, die gewährleisten, dass Sie Ihre Daten bei einem Laufwerkausfall oder Benutzerfehler abrufen können. Zu den Sicherungslösungen gehören derzeit NAS, EVault Backup und R1Soft CDP; alle diese Lösungen sind in einer Vielzahl von Speicheroptionen verfügbar.
Sie können einen der folgenden Backup-Services auswählen, um Ihre Daten an einer sicheren Position zu speichern: 
  * EVault Backup ist ein automatisiertes, agentenbasiertes Sicherungssystem. Dies ist eine gängige, komfortable und wartungsfreie Lösung zur Verwaltung Ihres Geräts. Sie ist kompatibel mit Microsoft-Software, einschließlich Exchange und SQL (über zusätzliche Plug-ins). EVault-Benutzer interagieren mit diesem Service über die webbasierte EVault-Anwendung WebCC.
  * R1Soft Continuous Data Protection (CDP) kann auf Ihrem Server oder auf der selbstverwalteten virtuellen Maschine installiert werden. Diese Lösung empfiehlt sich, wenn Sie nach einer einzigen Schnittstelle zum Verwalten all Ihrer Sicherungen suchen. Sie interagieren mit R1Soft CDP über Ihr proprietäres Managementsystem, das die Installation von Agenten auf virtuellen Maschinen ermöglicht und Datenbank-Plug-ins für zusätzliche Funktionalität bietet.

 Weitere Informationen zu den einzelnen Sicherungslösungen können Sie dem Abschnitt [Speicher ![Symbol für externen Link](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} entnehmen und weitere Informationen zum Sichern Ihrer Daten erhalten Sie im Abschnitt [Einführung in Backup-Services](/docs/infrastructure/Backup/index.html). 

### Redundanz nicht voraussetzen, sondern sicherstellen
{: #cp_bpknowredundant}

Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur bietet mehrere Add-on-Redundanzen, die doppelte Pfade, redundante Stromversorgungssysteme und RAID-Konfigurationen umfassen. Vergewissern Sie sich, dass Sie eine oder mehrere dieser Funktionen bereitgestellt haben, damit sichergestellt ist, dass Sie in einer redundanten Umgebung arbeiten und im Fall einer Störung geschützt sind.

### Sicherung der Informationen vor einem erneuten Laden des Betriebssystems überprüfen
{: #cp_bpnoperfOSwobackupconf}

Beim erneuten Laden des Betriebssystems werden alle Daten von der Festplatte des Geräts entfernt. Bevor Sie das erneute Laden des Betriebssystems einleiten, müssen Sie Ihre Informationen sichern und den Erfolg der Sicherung verifizieren, damit keine Daten verlorengehen. Nachdem einem erneuten Laden des Betriebssystem können verlorene Informationen nicht mehr abgerufen werden.

## Adaptec Storage Manager (ASM) nicht entfernen
{: #cp_bpsupdontremovasm}

 Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur verwendet ASM, um den Status Ihres RAID-Arrays zu überwachen. Falls Sie diese Software löschen, ist das Support-Team nicht in der Lage, Ihr Gerät zu überwachen. Wenn ASM von einem Gerät entfernt wurde, sind keine RAID-Fehleralerts für das Gerät verfügbar und Sie werden nicht vom automatischen Benachrichtigungssystem über den Fehler informiert.
