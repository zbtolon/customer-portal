---

copyright:

  years: 2018

lastupdated: "2018-05-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Zwei-Faktor-Authentifizierung einrichten
{: #customerportal_2fa}

Im Kundenportal können Sie die externe Zwei-Faktor-Authentifizierung (2FA) aktivieren, um für die Anmeldung beim Portal einen zusätzlichen Schutz bereitzustellen. Diese zusätzliche Sicherheitsebene schützt das Konto vor einem nicht verifizierten Zugriff und gewährleistet somit den Schutz von Geräten, Daten und Kontoinformationen. {:shortdesc}

Wenn Sie die 2FA im Kundenportal für Ihr vorhandenes SoftLayer-Konto aktivieren, müssen Sie bei der Anmeldung an der {{site.data.keyword.Bluemix_notm}}-Konsole Ihren Sicherheitscode eingeben. Allerdings gilt die 2FA nur für die Infrastrukturressourcen in Ihrem {{site.data.keyword.Bluemix_notm}}-Konto. Es kann folglich sein, dass Sie diverse Aktionen für die Ressourcen in Ihrem {{site.data.keyword.Bluemix_notm}}-Konto ausführen können, ohne die 2FA abzuschließen. 

Die Zwei-Faktor-Authentifizierung für Ihr SoftLayer-Konto erfolgt nicht pro IBMid. Sie erfolgt weiterhin pro Konto. Wenn eine IBMid mehreren Konten zugeordnet ist und Sie zwischen den Konten wechseln, müssen Sie Ihre Identität bei jedem Wechsel zu einem anderen Konto bestätigen. Dies gilt sogar dann, wenn das vorherige Konto und das neue Konto beide mit demselben 2FA-Verfahren konfiguriert sind.

## 2FA aktivieren

Es gibt zwei Arten von Zwei-Faktor-Authentifizierung. Beide Methoden der externen Authentifizierung können gegen eine geringe monatliche Gebühr für jeden Benutzer hinzugefügt werden. 

* Symantec Identity Protection ist unser am häufigsten genutztes Tool für die externe Authentifizierung. Es stellt beim Zugriff auf das Kundenportal zusätzlich zum Benutzernamen und Kennwort einen dynamischen Sicherheitscode bereit. 
* Die Authentifizierung mit PhoneFactor stellt eine externe Benutzerauthentifizierung mittels Telefon, SMS oder mobiler App bereit. 

 Wenn Sie über ein verknüpftes Konto verfügen, können Sie die Einstellung für die Mehrfaktorauthentifizierung nutzen, indem Sie die [Mehrfaktorauthentifizierung](/docs/iam/mfa.html) für Ihr gesamtes {{site.data.keyword.Bluemix_notm}}-Konto aktivieren.
 {: tip}

Führen Sie die folgenden Schritte aus, um die Zwei-Faktor-Authentifizierung einzurichten: 

1. Greifen Sie auf den Bildschirm **Benutzer** im Kundenportal zu.  
2. Wählen Sie im Menü **Aktionen** für den gewünschten Benutzer **Externe Authentifizierung hinzufügen** aus. 
3. Führen Sie basierend auf dem Typ der gewünschten externen Authentifizierung die folgenden Schritte aus: 
    * Wenn Sie sich für Symantec Identity Protection entscheiden, wählen Sie **Symantec Identity Protection** aus und geben Sie dann die Berechtigungs-ID des Benutzers ein. 
    * Wenn Sie sich für PhoneFactor entscheiden, wählen Sie **PhoneFactor** aus. 
4. Klicken Sie auf **Weiter**.
5. Füllen Sie die Bedienerführungen im Bildschirm für den Werbeaktionscode und die MSA-Bestätigung aus. 
6. Klicken Sie auf **Externe Authentifizierung bestellen**, um die Bestellung abzuschließen. Klicken Sie auf **Abbrechen**, um die Aktion abzubrechen. 

## Nächste Schritte
{: #2fanextsteps}

Nachdem Sie die externe Authentifizierung für einen Benutzer hinzugefügt haben, richtet sich der nächste Schritt nach dem Authentifizierungstyp.
* Falls Sie 'Symantec Identity Protection' aktiviert haben, müssen Sie den Sicherheitscode hinzufügen, der der Berechtigungsnachweis-ID des Benutzers zugeordnet ist, die im System eingegeben wurde, als Symantec Identity Protection zum Konto hinzugefügt wurde.
* Falls Sie 'PhoneFactor' aktiviert haben, muss der Benutzer PhoneFactor aktivieren, um diesen Typ der Zwei-Faktor-Authentifizierung für das Konto zu verwenden. 

### PhoneFactor-Authentifizierung aktivieren
{: #cp_actphonefacauth}

Nachdem Sie PhoneFactor hinzugefügt haben, müssen Sie die externe Authentifizierung mit PhoneFactor manuell über das Kundenportal aktivieren. Da PhoneFactor einen manuellen Kontakt verwendet, muss unbedingt sichergestellt sein, dass alle dem Konto zugeordneten Telefonnummern jederzeit aktuell sind. Nicht aktualisierte Kontaktinformationen könnten dazu führen, dass der Zugriff auf das Kundenportal und VPN nicht möglich ist, wenn PhoneFactor aktiv ist. Nachdem PhoneFactor erfolgreich hinzugefügt wurde, erhalten Sie eine E-Mail zur Bestätigung, dass PhoneFactor hinzugefügt worden ist. Nach dem Empfang der E-Mail führen Sie die folgenden Schritte aus, um die PhoneFactor-Authentifizierung zu aktivieren.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto > Benutzer** aus.
3. Klicken Sie auf den Benutzernamen, um auf das zugehörige Benutzerprofil für diesen Benutzer zuzugreifen.
4. Blättern Sie zum Abschnitt **PhoneFactor-Einstellungen**.

  Falls der Abschnitt 'PhoneFactor-Einstellungen' nicht verfügbar ist, überprüfen Sie zuerst, ob Sie die Bereitstellungs-E-Mail für PhoneFactor erhalten haben, in der angegeben ist, dass PhoneFactor bereitgestellt wurde. Falls PhoneFactor bereitgestellt wurde und der Abschnitt nicht verfügbar ist, erstellen Sie ein Support-Ticket. Wurde PhoneFactor noch nicht bereitgestellt, warten Sie, bis Sie die E-Mail erhalten haben, und wiederholen Sie den Versuch.
  {: tip}

5. Wählen Sie in der Liste **Status** den Eintrag **Aktiv** aus.
6. Bearbeiten Sie die **Primäre Telefonnummer** für die Authentifizierung.
  1. Klicken Sie auf den Link **Bearbeiten**.
  2. Geben Sie in den entsprechenden Feldern den **Landescode**, die **Telefonnummer** und gegebenenfalls die **Durchwahl** ein.
  3. Klicken Sie auf **Nummer authentifizieren und speichern**, um die Authentifizierung abzuschließen.

    Wenn Sie eine Telefonnummer für die Authentifizierung hinzufügen, muss sich das Telefon in Ihrer Nähe befinden. Nachdem Sie auf **Authentifizieren** geklickt haben, wird die Nummer angerufen und Sie werden aufgefordert, einen Schritt zur Authentifizierung der Nummer auszuführen. Telefonnummern können ohne eine Ausführung dieser Schritte nicht authentifiziert werden.
    {: tip}

  4. Wiederholen Sie diese Schritte, um eine **sekundäre Telefonnummer** hinzuzufügen.
7. Wählen Sie in der Liste **Methode** den Eintrag **Kontaktmethode** aus.
8. Wählen Sie in der Liste **PIN-Typ** einen **PIN-Typ** aus.
9. Falls Sie **Einmalig** > **PIN-Wert** auswählen, geben Sie die PIN im Feld **PIN-Wert** ein.
10. Klicken Sie auf **Aktualisieren**, um die Änderungen zu aktualisieren und die PhoneFactor-Authentifizierung zu aktivieren.

Nach der Aktivierung von PhoneFactor ist für das Kundenportal oder das VPN eine Authentifizierung über PhoneFactor erforderlich. Nachdem Sie sich mit den Benutzerberechtigungsnachweisen authentifiziert haben, wird Ihnen in einer Nachricht mitgeteilt, dass ein Versuch für die PhoneFactor-Authentifizierung erfolgt. Sie selbst oder der Benutzer, den Sie hinzufügen, muss sich in der Nähe des für PhoneFactor angegebenen Telefons befinden, um die Authentifizierung abschließen zu können. PhoneFactor unternimmt fünf Authentifizierungsversuche. Nach fünf erfolglosen Authentifizierungsversuchen werden Sie für ca. eine Stunde gesperrt. Sie können die Einstellungen für die PhoneFactor-Authentifizierung jederzeit ändern; dies kann auch durch einen Benutzer mit Verwaltungszugriff auf das Konto vorgenommen werden.  Eine Inaktivierung von PhoneFactor kann jederzeit durch Sie selbst oder einen Administrator des Kontos erfolgen.

 Wenn Sie PhoneFactor für das Kundenportal und Ihre VPN-Anmeldung einrichten, findet die Zwei-Faktor-Authentifizierung für beide separat statt.
 {: tip}

#### Methoden für die PhoneFactor-Authentifizierung
{: #cp_phonefacauthmeths}

Falls Sie PhoneFactor als Authentifizierungstyp festlegen, können Sie eine der folgenden Optionen als Authentifizierungsmethode auswählen:

<dl>
<dt>Anruf und Standardwert (ohne PIN)</dt>
<dd>Wenn diese Option aktiviert ist, empfangen Sie einen Anruf unter der aktivierten primären Nummer, sobald Sie sich beim Portal anmelden. Wenn Sie den Anruf annehmen, werden Sie aufgefordert, die Raute-Taste (#) zu drücken, um die Authentifizierung abzuschließen.</dd>
<dt>Anruf mit PIN</dt>
<dd>Wenn diese Option ausgewählt ist, geben Sie einen PIN-Wert im Kundenportal ein. Die PIN muss 4 bis 8 Ziffern umfassen. Sobald Sie versuchen, sich beim Portal anzumelden, empfangen Sie einen Anruf unter der im Portal aufgelisteten primären Nummer. Wenn Sie den Anruf annehmen, werden Sie aufgefordert, Ihre PIN einzugeben und die Raute-Taste (#) zu drücken, um die Authentifizierung abzuschließen.</dd>
<dt>SMS-Text und einmalige PIN</dt>
<dd>Wenn diese Option ausgewählt ist, empfangen Sie eine Textnachricht mit einer PIN, die Sie zur Beantwortung der Nachricht verwenden. Nachdem Sie die bereitgestellte PIN eingegeben haben, wird der Authentifizierungsprozess abgeschlossen und Sie werden beim Portal angemeldet.</dd>
<dt>SMS-Text mit Einmalanmeldung &amp; PIN-Wert</dt>
<dd>Wenn diese Option ausgewählt ist, erstellen Sie einen PIN-Wert aus 4 bis 8 Ziffern. Anschließend empfangen Sie eine Textnachricht und antworten mit dem bereitgestellten Code sowie Ihrer PIN-Nummer ohne Leerzeichen.</dd>
<dt>PhoneFactor-App und Standardwert (ohne PIN)</dt>
<dd>Öffnen Sie die PhoneFactor-Anwendung (Microsoft Authenticator) auf Ihrem Gerät und klicken Sie auf <strong>Authentifizieren</strong>. Es wird die Nachricht ausgegeben, dass Sie sich erfolgreich mit PhoneFactor authentifiziert haben, und Sie werden beim Portal angemeldet.</dd>
<dt>PhoneFactor-App mit PIN</dt>
<dd>Bei dieser Option legen Sie im Portal eine PIN aus 4 bis 8 Ziffern fest. Anschließend rufen Sie die PhoneFactor-Anwendung (Microsoft Authenticator) auf Ihrem Gerät auf. Danach geben Sie Ihre im Portal erstellte PIN ein und klicken auf <strong>Authentifizieren</strong>, um sich beim Portal anzumelden.</dd>
</dl>
