---

copyright:

  years: 1994, 2018

lastupdated: "2018-07-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Kennwörter verwalten
{: #customerportal_manpws}

Als Masterbenutzer oder Eigner eines Kontos können Sie die Kennwortaufzeichnung aktivieren und auch ein Kennwort für den einmaligen Zugriff auf das Konto einrichten. Die Kennwortaufzeichnung ermöglicht Benutzern die Speicherung von Softwarekennwortdaten für Geräte und deren zugehörige Software.
{:shortdesc}

## Kennwortaufzeichnung aktivieren
{: #customerportal_enabpwtrak}

Das Kundenportal enthält ein optionales Tool für die [Kennwortaufzeichnung ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/devices/passwords){:new_window}, das für jedes Konto verwendet werden kann. Benutzer können ihre Benutzernamen und Kennwörter mithilfe des Tools abrufen, falls die Informationen vergessen wurden oder verloren gegangen sind.

Die Kennwortaufzeichnung wird auch von Support-Teams genutzt, falls ein Fernzugriff auf ein System erforderlich ist. Benutzernamen und Kennwörter werden vom Support nur bei Bedarf und bei bestehender Berechtigung zur Ticketauflösung verwendet.

Die Aufzeichnung von Kennwörtern im Kundenportal ist optional. Jeder Benutzer mit den entsprechenden Berechtigungen kann alle von diesem Tool aufgezeichneten Kennwörter anzeigen. Benutzer- und Kennwortinformationen werden manuell aufgezeichnet und sind daher nicht automatisch mit einem Gerät oder seiner Software synchronisiert. Denken Sie daher daran, bei einer Aktualisierung von Benutzern und Kennwörtern auf Geräten und in Software auch das Tool für die Kennwortaufzeichnung zu aktualisieren. Führen Sie zum Hinzufügen eines Benutzers zum Tool für die Kennwortaufzeichnung die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie im Menü die Optionen **Geräte** > **Verwalten** > **Kennwörter** aus.
3. Klicken Sie auf die Registerkarte **Berechtigungsnachweise hinzufügen**.
4. Wählen Sie den **Namen des Geräts**, dem der Benutzer zugeordnet ist, in der Dropdown-Liste **Gerätename** aus.
5. Wählen Sie die **Software**, der der Benutzer zugeordnet ist, in der Dropdown-Liste **Software** aus.

  Die aufgelistete Software wird durch die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur über gebührenpflichtige oder kostenlose Abonnements bereitgestellt. Die Aufzeichnung über das Kundenportal ist nicht für Software anderer Anbieter verfügbar, die manuell auf dem Gerät installiert wurde.
  {: tip}

6. Geben Sie den Benutzernamen und das Kennwort für die Software in den entsprechenden Feldern ein.
8. Optional können Sie etwaige maßgebliche Kommentare im Feld **Hinweise** eingeben.
9. Klicken Sie auf **Berechtigungsnachweise hinzufügen**.

Nachdem Sie den Benutzer zum Tool für die Kennwortaufzeichnung hinzugefügt haben, werden die Informationen so lange im Tool gespeichert, bis sie manuell gelöscht werden. Alle Benutzernamen- und Kennwortkombinationen werden standardmäßig basierend auf dem Gerätenamen gespeichert. Einträge werden zunächst nach dem Gerätenamen und dann nach dem Benutzernamen alphabetisch sortiert angezeigt.

### Informationen im Tool für die Kennwortaufzeichnung filtern
{: #cp_filterusinfopwtracktool}

Um Benutzerinformationen im Tool für die Kennwortaufzeichnung anzuzeigen, zu bearbeiten oder zu löschen, können Sie mithilfe eines Filters schnell nach einem Benutzer suchen. Das Filtern bei der Suche nach einem Benutzer ist hilfreich, wenn die Liste der Benutzer mehrere Zeilen oder Seiten umfasst. Führen Sie zum Filtern nach Gerät, Software oder Benutzer im Tool für die Kennwortaufzeichnung die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie im Menü die Optionen **Geräte** > **Verwalten** > **Kennwörter** aus.
3. Klicken Sie auf die Registerkarte **Filtern**.
4. Wählen Sie den Gerätenamen, die Software oder den Benutzernamen im entsprechenden Feld aus bzw. geben Sie den Wert dort ein.
5. Klicken Sie auf **Filtern**.

Sie können die Benutzerinformationen auswählen, die Sie anzeigen, bearbeiten oder entfernen wollen.

### Benutzerinformationen im Tool für die Kennwortaufzeichnung bearbeiten
{: #cp_editusinfopwtracktool}

Nachdem Sie einen Benutzer zum Tool für die Kennwortaufzeichnung hinzugefügt haben, können Sie die Details bearbeiten, die dem Benutzer oder dem Kennwort zugeordnet sind. Führen Sie zum Bearbeiten von Informationen für einen Benutzer im Tool für die Kennwortaufzeichnung die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie im Menü die Optionen **Geräte** > **Verwalten** > **Kennwörter** aus.
3. Suchen Sie im Tool nach der gewünschten Kombination aus Gerät und Benutzer. Mit der Filterfunktion können Sie die Suche nach einem Benutzer beschleunigen.
4. Klicken Sie auf eine Stelle der Zeile, um die Ansicht mit den Benutzerdetails zu öffnen.
5. Aktualisieren Sie das Feld **Benutzername** oder **Kennwort** wie gewünscht.
6. Klicken Sie auf **Speichern**, um Ihre Änderungen zu speichern.

Nachdem Sie einen Benutzer oder ein Kennwort im Tool für die Kennwortaufzeichnung bearbeitet haben, werden die Informationen unmittelbar aktualisiert.

## Konto für Zugriff mit Einmalkennwort konfigurieren
{: #cp_confportacc1timpwacc}

Damit Sie das Konto konfigurieren können, müssen Sie zuerst die Verisign-Anwendung 'VIP Access' einrichten. Falls 'VIP Access' noch nicht installiert und eingerichtet ist, laden Sie zunächst die Anwendung für eines der folgenden Geräte herunter:
* Telefon: [https://m.vip.symantec.com/home.v ![Symbol für externen Link](../icons/launch-glyph.svg)](https://m.vip.symantec.com/home.v){:new_window}
* Desktop: [https://idprotect.verisign.com/desktop/download.v ![Symbol für externen Link](../icons/launch-glyph.svg)](https://idprotect.verisign.com/desktop/download.v){:new_window}

Gehen Sie anschließend wie folgt vor:
1. Öffnen Sie die Anwendung. Suchen Sie die Berechtigungsnachweis-ID und Ihr aktuelles Einmalkennwort. Das Kennwort können Sie zunächst ignorieren, aber die Berechtigungsnachweis-ID benötigen Sie für das Portal. Lassen Sie daher die Anwendung geöffnet.
2. Melden Sie sich beim Kundenportal als der Benutzer an, für den Sie das Einmalkennwort konfigurieren wollen.
3. Klicken Sie auf **Konto** > **Benutzer** > **Aktionen** > **Externe Authentifizierung hinzufügen**.
4. Wählen Sie den Typ der Authentifizierung aus, die Sie hinzufügen wollen. Wenn Sie die Verisign-Anwendung verwenden, wählen Sie **Symantec Identity Protection** aus.
5. Geben Sie die in Schritt 1 ermittelte Berechtigungsnachweis-ID ein und klicken Sie auf **Weiter**.
6. Schließen Sie den Bestellablauf ab. Ihre zusätzliche Sicherheitsoption wird in nur wenigen Minuten automatisch angewendet.
7. Wählen Sie nach einigen Minuten in der Navigationsleiste die Optionen **Konto** > **Benutzer** aus und wählen Sie den Benutzer aus, für den Sie das Einmalkennwort konfiguriert haben.
8. Klicken Sie auf den Link **Berechtigungsnachweis aktualisieren** im Abschnitt **Symantec-Validierungseinstellungen**.
9. Wählen Sie die Einstellung **Aktiviert** bei **Berechtigungsnachweisstatus** aus und klicken Sie auf **Berechtigungsnachweis aktualisieren**.
10. Nachdem die zusätzliche Sicherheitsoption erfolgreich verarbeitet worden ist, können Sie sich wie gewohnt beim Kundenportal anmelden. Nach Übergabe Ihres Benutzernamens und Ihres Kennworts werden Sie zur Eingabe eines Sicherheitscodes aufgefordert.
11. Öffnen Sie die Anwendung 'Verisign Identity Protection' auf dem bevorzugten Gerät und geben Sie den angezeigten Code ein, um sich anzumelden.

Bewahren Sie Ihre ursprüngliche Berechtigungsnachweis-ID für Verisign Identity Protection für den Fall, dass Sie sie zu einem späteren Zeitpunkt benötigen, an einem sicheren Ort auf. Ohne diese ID können Sie nicht auf das Portal zugreifen.

## Ihr Kennwort zurücksetzen
{: #cp_reset-your-password}

Die Vorgehensweise zum Zurücksetzen Ihres Kennworts basiert darauf, ob zur Authentifizierung bei der Anmeldung an Ihrem Konto eine IBMid verwendet wird.  

### Kennwort eines IBMid-Kontos zurücksetzen
{: #cp_reset-IBMid-password}

Wenn Sie zur Authentifizierung eine IBMid verwenden, dann rufen Sie zum Zurücksetzen oder Wiederherstellen Ihres Kennworts Ihr IBMid-Profil auf und führen Sie die im Abschnitt **Anmelden** aufgeführten Anweisungen aus.

### Kennwort eines Kontos zurücksetzen
{: #cp_reset-password}

Wenn Sie zur Kontoauthentifizierung keine IBMid verwenden, dann müssen Sie die folgenden Schritte ausführen:

1. Klicken Sie auf der Anmeldeseite im [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} auf den Link für ein verlorenes Kennwort.
2. Wenn Sie dazu aufgefordert werden, geben Sie Ihren aktuellen Benutzernamen ein.
3. Überprüfen Sie, ob Sie eine E-Mail mit einer Nachricht erhalten haben, die einen Link zum Zurücksetzen Ihres Kennworts enthält. Dieser Link ist für einen Zeitraum von 24 Stunden gültig.
4. Wählen Sie drei Sicherheitsfragen aus und beantworten Sie sie.

Sie haben fünf Versuche zur Beantwortung der Sicherheitsfragen. Bei mehr als fünf Versuchen wird das Formular zum Zurücksetzen des Kennworts für 15 Minuten gesperrt, bevor Sie es erneut versuchen können.

Informationen zum Arbeiten mit VPN-Kennwörtern finden Sie im Abschnitt zum [Aktualisieren des VPN-Kennworts eines Benutzers](/docs/infrastructure/iaas-vpn/update-password.html#update-a-user-s-vpn-password).
{: tip}
