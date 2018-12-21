---

copyright:

  years: 1994, 2018

lastupdated: "2018-10-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# Systemereignisse in der {{site.data.keyword.Bluemix_notm}}-Infrastruktur überwachen
{: #customerportal_monevent}

Durch die Überwachung von Systemereignissen können Sie für einen reibungslosen Betrieb Ihrer Systeme sorgen. Informationen zum Konfigurieren und Verwalten von virtuellen Servern in der {{site.data.keyword.BluSoftlayer_full}}-Infrastruktur finden Sie unter [Einführung in virtuelle Server](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers).
{:shortdesc}

## Prüfprotokoll für ein Konto anzeigen
{: #cp_viewacctauditlog}

Jedes Kundenportalkonto wird zusammen mit einem Prüfprotokoll bereitgestellt, in dem die Interaktionen jedes Benutzers im Kundenportal aufgezeichnet werden. Zu den aufgezeichneten Interaktionen gehören Anmeldeversuche (erfolgreich und erfolglos), Aktualisierungen der Portgeschwindigkeit, Systemstarts oder -beendigungen und Warmstarts sowie diejenigen Interaktionen, die von den Mitarbeitern des Support-Teams für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur ausgeführt werden. Führen Sie die folgenden Schritte aus, um ein Prüfprotokoll für ein Benutzerkonto anzuzeigen.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto** > **Verwalten** > **Prüfprotokoll** aus, um auf das Prüfprotokoll zuzugreifen.

Im Prüfprotokoll werden anfangs die letzten 25 Interaktionen von Benutzern mit dem Konto angezeigt. Sie können jederzeit bis zu 200 Interaktionen anzeigen. Die Anzahl der angezeigten Ergebnisse können Sie in der Dropdown-Liste **Anzeigen** aktualisieren. Falls Einstellungen geändert wurden, enthält die Spalte **Aktion** für die Interaktion einen Link. Klicken Sie auf einen dieser Links, um die durch die Aktion beeinflusste Einstellung sowie Details über die Änderung anzuzeigen. Wenn Sie auf den Gerätenamen oder Benutzernamen für eine Interaktion klicken, werden Sie zur Anzeige mit den Gerätedetails bzw. zur Anzeige mit dem Benutzerprofil weitergeleitet.

## Zugriffsprotokoll eines Benutzers anzeigen
{: #cp_viewuserlogs}

Zugriffsprotokolle zeigen Daten für jeden Zugriffsversuch an, der durch einen bestimmten Kundenportalbenutzer unternommen wurde. In den Protokollen sind für jeden Zugriffsversuch eine Datums-und Zeitmarke und eine IP-Adresse angegeben. Führen Sie die folgenden Schritte aus, um das Zugriffsprotokoll eines Benutzers anzuzeigen.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} zu.
2. Wählen Sie in der Menüleiste die Optionen **Konto** > **Benutzer** aus, um auf das Fenster 'Benutzer' zuzugreifen.
3. Wählen Sie in der Dropdown-Liste **Aktionen** den Eintrag **Prüfprotokoll anzeigen** aus, um das Zugriffsprotokoll des Benutzers anzuzeigen.

Im Zugriffsprotokoll werden für jeden Benutzer die von ihm unternommenen Zugriffsversuche nach Datum sortiert zusammen mit der IP-Adresse angezeigt, über die der Zugriffsversuch erfolgte. Die Informationen im Zugriffsprotokoll sind schreibgeschützt, sodass zu keinem Zeitpunkt Änderungen am Inhalt vorgenommen werden können. Sie können das Zugriffsprotokoll jederzeit erneut anzeigen, indem Sie die obigen Schritte wiederholen. Um die Protokolle zu verlassen und zur Anzeige 'Benutzer' zurückzukehren, klicken Sie auf den Link **Alle Benutzer anzeigen**.
