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


# Benutzerprofil verwalten
{: #customerportal_accuserprof}

Im Kundenportal enthält ein Benutzerprofil eine Vielzahl von Daten über den Benutzer, inklusive Kontaktinformationen und API-Schlüssel. An dieser Stelle werden auch Kennwörter gespeichert. Falls Sie Verwaltungszugriff besitzen, können Sie über das Profil die Berechtigungen und den Gerätezugriff ändern.
{:shortdesc}

Innerhalb des Benutzerprofils können Sie Kontaktinformationen und Kennwörter verwalten, API-Schlüssel anzeigen sowie Berechtigungen und den Gerätezugriff auf der Grundlage Ihrer Berechtigungen aktualisieren.

## Benutzerprofil bearbeiten
{: #cp_edituserprofile}

Nachdem ein Benutzerprofil im Kundenportal erstellt wurde, können Sie es jederzeit bearbeiten. Zu den Details eines Benutzerprofils gehören persönliche Informationen, Anmeldeeinstellungen, API-Zugriffsdetails, Abonnements von Benutzerbenachrichtigungen und  Sicherheitsfragen. Führen Sie zum Bearbeiten eines Benutzerprofils die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto > Benutzer** aus.
3. Klicken Sie auf den Benutzernamen, um auf das zugehörige Benutzerprofil für diesen Benutzer zuzugreifen.
4. Bearbeiten Sie die Details für das **Benutzerprofil** wie gewünscht. Für Benutzer in Konten, die die IBMid für die Authentifizierung verwenden, aktualisieren Sie Ihre E-Mail-Adresse und Ihr Kennwort im IBMid-Profil. Weitere Informationen können Sie Tabelle 1 entnehmen.
5. Falls Sie Ihr Kennwort nach der Anmeldung zurücksetzen wollen, klicken Sie auf **Kennwort zurücksetzen**, um eine E-Mail zu erstellen, die Ihnen die Änderung Ihres Kennworts ermöglicht.
6. Klicken Sie auf **Benutzer bearbeiten**, um die Änderungen zu übergeben.

| Feld | Definition |
|-----|----------|
| Vorname, Nachname | Der Vor- und Nachname des Benutzers, der dem Benutzerprofil zugeordnet ist.|
| E-Mail-Adresse | Die bevorzugte E-Mail-Adresse für den Empfang von Benachrichtigungen bezüglich des Kontos aus der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur. Eine Änderung der E-Mail-Adresse ändert den Datensatz in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur. Auf die Verknüpfung mit den IBMid-Authentifizierungsnachweisen hat diese Änderung keinen Einfluss. Die E-Mail-Adresse für die IBMid müssen Sie im IBMid-Profil ändern.|
| Zeitzone | Die bevorzugte Zeitzone für das Anzeigen von Daten mit Zeitmarken.|
| Telefon, Telefon (alternativ)| Die bevorzugten Telefonnummern für Ansprechpartner, die von der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur verwendet werden sollen.|
| Straße, Stadt, Land, Bundesland/Kanton, Postleitzahl | Die vollständige Adresse für Ansprechpartner, die von der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur verwendet werden soll.|
{: caption="Tabelle 1. Konfigurationseinstellungen für persönliche Informationen zur Bearbeitung eines Benutzerprofils" caption-side="top"}

|Feld|Definition|
|-----|----------|
| Zugriff auf IP beschränken | Die IP-Adresse, auf die der Zugriff beschränkt werden soll, wenn versucht wird, das Kundenportal unter dem zugeordneten Benutzerprofil zu verwenden. |
| Kennwortablauf in (nur für Benutzer in Konten, die zur Authentifizierung NICHT die IBMid verwenden) | Der Zeitraum, für den ein Kennwort dem Benutzerprofil zugeordnet sein soll, bevor ein neues Kennwort ausgewählt werden muss. |
| Übergeordneter Benutzer | Das Benutzerkonto, das als übergeordneter Benutzer des Benutzerprofils gilt. Der Standardwert für den übergeordneten Benutzer ist die primäre Konto-ID. |
| Sicherheitsfragen erforderlich? | Wählen Sie dieses Kontrollkästchen aus, wenn bei der Anmeldung Sicherheitsfragen erforderlich sein sollen. Falls dieses Kästchen ausgewählt ist, sind Sicherheitsfragen für das Benutzerprofil erforderlich. |
| VPN-Kennwort | Das Kennwort, das für den VPN-Zugriff verwendet werden soll. Klicken Sie auf das Kontrollkästchen **Portalkennwort für VPN verwenden**, um das Kundenportalkennwort für den Zugriff auf das {{site.data.keyword.BluSoftlayer_notm}}-Infrastrukturnetz über VPN zu verwenden. |
{: caption="Tabelle 2. Konfigurationseinstellungen für Anmeldeeinstellungen zur Bearbeitung eines Benutzerprofils" caption-side="top"}

|Abschnitt|Feld|Definition|
|-------|-----|----------|
| API-Zugriffsinformationen | Zulässige IPs | Die IP-Adressen, die für die Authentifizierung bei der API unter Verwendung des eindeutigen API-Schlüssels, der dem Benutzerprofil zugeordnet ist, zulässig sind. |
| Abonnements von Benutzerbenachrichtigungen | Abrechnung | Wählen Sie das Kontrollkästchen **Abrechnung** aus, um eine Rechnung per E-Mail zu erhalten, nachdem sie erstellt wurde. |
| Sicherheitsfragen | Sicherheitsfrage | Bei der Bearbeitung des Profils müssen Sie diese Frage beantworten, um sich anzumelden, wenn Sicherheitsfragen für Ihr Profil aktiviert wurden.
| Sicherheitsantworten | Antwort | Die Antwort auf die maßgebliche Sicherheitsfrage. Die Groß-/Kleinschreibung muss beachtet werden. |
{: caption="Tabelle 3. Weitere Konfigurationseinstellungen zur Bearbeitung eines Benutzerprofils" caption-side="top"}
Nachdem Sie Bearbeitungen eines Benutzerprofils übergeben haben, werden die Änderungen sofort angewendet. Sie können das Benutzerprofil jederzeit erneut ändern, indem Sie die obigen Schritte wiederholen.

Weitere Informationen zum Einrichten eines IBMid-Kontos finden Sie im Abschnitt [Zur IBMid wechseln](/docs/account/softlayerlink.html#switching-to-ibmid).

## Berechtigungen eines Benutzers für das Kundenportal bearbeiten
{: #cp_editusercpperm}

Die Benutzerberechtigungen im Kundenportal werden durch den Kontoadministrator beim Hinzufügen des Benutzers festgelegt und können jederzeit durch einen berechtigten Benutzer geändert werden. Sie können Ihr eigenes Benutzerprofil und - als Benutzer mit Verwaltungsaufgaben - einige Felder der Benutzerprofile von Benutzern bearbeiten, die Sie hinzugefügt haben. Die Berechtigungen sind auf fünf Registerkarten (Support, Geräte, Netz, Services, Konto) verteilt. Sie können die Berechtigungen jeweils für einen einzigen Benutzer zur Zeit aktualisieren und müssen die Änderungen speichern, damit sie wirksam werden.

Führen Sie zum Bearbeiten der Berechtigungen eines Benutzers für das Kundenportal die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto > Benutzer** aus.
3. Klicken Sie auf den Benutzernamen, um auf das Benutzerprofil zuzugreifen.
4. Klicken Sie auf das Symbol **Berechtigungen**, um auf das Fenster 'Berechtigungen' zuzugreifen.

  Möglicherweise wird die Nachricht ausgegeben, dass Änderungen nicht im Benutzerprofil gespeichert wurden. Falls keine Änderungen am Profil vorgenommen wurden, können Sie mittels Clickthrough die Änderungen verwerfen und auf das Fenster 'Berechtigungen' zugreifen.
  {: tip}

5. Wählen Sie die Berechtigungen aus:
  * Um Schnellberechtigungen festzulegen, wählen Sie das Berechtigungsset in der Liste **Schnellberechtigungen** aus. Nachdem Sie ein Berechtigungsset ausgewählt haben, werden alle Berechtigungen die dem Set zugeordnet sind, in orangefarbigem Text mit einem orangefarbigen Pfeil angezeigt, der auf das Kontrollkästchen zeigt. Klicken Sie dann für jede Registerkarte auf **Berechtigungen festlegen**.
  * Um einzelne Berechtigungen festzulegen, wählen Sie jedes Kontrollkästchen auf den Registerkarten aus bzw. ab, damit die Berechtigungen des Benutzers aktualisiert werden. Klicken Sie auf einer Registerkarte auf **Alle Berechtigungen auswählen** oder **Alle Berechtigungen abwählen**, um alle Berechtigungen auf einmal aus- oder abzuwählen.
6. Klicken Sie auf **Portalberechtigungen bearbeiten**, um Änderungen zu übergeben und die Berechtigungen des Benutzers zu aktualisieren.
7. Wenn Sie die Berechtigungen des Benutzers auf die ursprünglichen Einstellungen zurücksetzen wollen, statt sie zu speichern, klicken Sie auf **Berechtigungen zurücksetzen**. Klicken Sie auf **Abbrechen**, um die Änderungen zu stornieren und zum Fenster 'Benutzer' zurückzukehren.

Benutzerberechtigungen werden sofort aktualisiert, nachdem Sie die Änderungen übergeben haben. Falls Berechtigungen erteilt wurden, kann der Benutzer die ausgewählten Funktionen anzeigen bzw. mit ihnen interagieren. Falls Berechtigungen entfernt wurden, kann der Benutzer die ausgewählten Funktionen nicht mehr anzeigen oder mit ihnen interagieren. Berechtigungen können jederzeit durch Wiederholung der obigen Schritte aktualisiert werden.

## Externe Authentifizierung für einen Benutzer hinzufügen
{: #cp_addextauthuser}

Ausgehend vom Kundenportal können Sie die externe Zwei-Faktor-Authentifizierung (2FA) aktivieren, um für die Anmeldung beim Portal Schutz bereitzustellen. Diese Sicherheitsebene schützt das Konto vor einem nicht verifizierten Zugriff und gewährleistet somit den Schutz von Geräten, Daten und Kontoinformationen. Weitere Informationen finden Sie unter [Zwei-Faktor-Authentifizierung einrichten](/docs/customer-portal/cpenable2fa.html#customerportal_2fa).


## Status eines Benutzers ändern
{: #cp_changeuserstat}

Ihr Status im Kundenportal bestimmt Ihre Zugriffsmöglichkeit auf das Kundenportal. Statuskategorien, die Sie für das Konto aktualisieren können, sind 'Aktiv', 'Inaktiviert' und 'Nur VPN'. Ihr Status kann sich aus einer Vielzahl von Gründen ändern und jederzeit aktualisiert werden. Die Statuskategorien für Kunden können von den Benutzern aktualisiert, aber auch automatisch aktualisiert werden. Hierzu gehören die folgenden Kategorien:
<dl>
<dt>Aktiv</dt>
<dd>Der Benutzer besitzt uneingeschränkten Zugriff auf das Kundenportal und das VPN gemäß den Berechtigungen, die durch den Kontoadministrator festgelegt wurden. Dieser Status kann jederzeit manuell ausgewählt oder geändert werden.</dd>
<dt>Inaktiviert</dt>
<dd>Der Benutzer besitzt keinen Zugriff auf Berechtigungen oder Abonnements für das Konto (inklusive Kundenportal und VPN). Falls die Statuskategorie durch einen anderen Benutzer im Konto auf 'Inaktiviert' gesetzt wird, kann dieser Status jederzeit manuell ausgewählt oder geändert werden.</dd>
<dt>Nur VPN</dt>
<dd>Der Benutzer besitzt uneingeschränkten Zugriff auf die VPN-Konnektivität gemäß seinen festgelegten Berechtigungen, kann jedoch nicht auf das Kundenportal zugreifen. Dieser Status kann jederzeit manuell ausgewählt oder geändert werden.</dd>
<dt>Inaktiv</dt>
<dd>Der Benutzer hat in den vergangenen 60 Tagen nicht auf das Kundenportal oder das VPN zugegriffen. Dieser Status wird vom System generiert.</dd>
<dt>Stornierung anstehend</dt>
<dd>Ein Administrator für das Konto hat diesen Benutzer storniert und die Stornierung wird gegenwärtig verarbeitet. Dieser Status wird vom System generiert.</dd>
</dl>

Führen Sie die folgenden Schritte aus, um den Status eines Benutzers im Kundenportal zu ändern.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto** > **Benutzer** aus.
3. Wählen Sie in der Liste **Aktionen** den Eintrag **Benutzerstatus ändern** aus.
4. Wählen Sie in der Liste **Status** den entsprechenden Status gemäß den Definitionen in der obigen Liste aus.
5. Klicken Sie auf **Speichern**.

Nachdem Sie den Status eines Benutzers aktualisiert haben, werden Änderungen an der Zugriffsmöglichkeit auf das Kundenportal am neuen Status ausgerichtet.


## VPN-Zugriff eines Benutzers bearbeiten
{: #cp_edituservpnaccess}

Wenn zu einem Kundenportalkonto ein [neuer Benutzer hinzugefügt wird](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct), wird der VPN-Zugriff unter einer Vielzahl von Verbindungsaufbaumethoden ausgewählt (inklusive SSL, PPTP oder einer Kombination dieser Verfahren). Beim VPN-Zugriff kann auf das gesamte private Netz zugegriffen werden oder der Netzzugriff auf eines oder mehrere bestimmte Teilnetz beschränkt werden. Sie können den VPN-Zugriff jederzeit im Fenster 'Benutzer' verwalten und aktualisieren. Führen Sie zum Bearbeiten des VPN-Zugriffs für einen Benutzer die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto** > **VPN-Zugriff** aus.
3. Klicken Sie in der Spalte **VPN-Zugriff** für den Benutzer auf den aktuellen VPN-Zugriffstyp, um das Fenster 'VPN-Zugriff' aufzurufen.
4. Wählen Sie in der Liste **VPN-Typ** eine VPN-Methode aus (SSL, PPTP, SSL und PPTP oder 'Keine'), die dem Benutzer zugeordnet werden soll.
5. Geben Sie an, wie Sie den **Teilnetzzugriff** verwalten wollen:
  * Wählen Sie **Automatisch** aus, damit der Teilnetzzugriff automatisch verwaltet wird.
  * Wählen Sie **Manuell** aus, um den Teilnetzzugriff manuell zu verwalten, und wählen Sie dann das Kontrollkästchen **Zugriff erteilen** für jedes Teilnetz aus, auf das der Benutzer Zugriff erhält. Achten Sie darauf, die Kontrollkästchen für all diejenigen Teilnetze abzuwählen, auf die der Benutzer keinen Zugriff haben soll.
6. Klicken Sie auf **Speichern**.

Nachdem Sie den VPN-Zugriff für einen Benutzer aktualisiert haben, werden seine Berechtigungen aktualisiert, und in der Spalte 'VPN-Zugriff' wird gegebenenfalls die aktualisierte VPN-Zugriffsmethode angezeigt.

### VPN-Zugriff aktivieren oder inaktivieren
{: #cp_pptpvpn}

Sie können das PPTP-VPN aktivieren, um einen sicheren Tunnel zum privaten Netz der {{site.data.keyword.BluSoftlayer_full}}-Infrastruktur zu bilden, die spezialisierte Client-Software verwendet, die auf Ihrem Desktop oder dem dedizierten Gerät ausgeführt wird. Sie können PPTP verwenden, wenn Sie Ihre gesamte Niederlassung verbinden müssen oder die VPN-Lösung mit SSL nicht verwenden können.

Ihnen wird eine PPTP-Verbindung mit zusätzlich verfügbaren Verbindungen zugeteilt. Sie können Unterstützung anfordern, um einen uneingeschränkten PPTP-Zugriff zu aktivieren, der ohne Aufpreis verfügbar ist. Führen Sie zum Aktivieren oder Inaktivieren des PPTP-VPN-Zugriffs die folgenden Schritte aus:

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Menüleiste die Optionen **Konto** > **VPN-Zugriff** aus.
3. Klicken Sie in der Spalte **VPN-Zugriff** für den Benutzer auf den aktuellen VPN-Zugriffstyp, um das Fenster 'VPN-Zugriff' aufzurufen.
4. Wählen Sie in der Liste **VPN-Typ** eine VPN-Methode aus (SSL, PPTP, SSL und PPTP oder 'Keine'), die dem Benutzer zugeordnet werden soll.


## E-Mail-Benachrichtigungen auswählen
{: #cp_select-email-notifications}

Sie können auswählen, welche E-Mail-Benachrichtigungen Sie von der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur empfangen wollen und welche nicht. Standardmäßig empfangen Sie alle E-Mail-Benachrichtigungen, aber Sie können diese Einstellung jederzeit ändern. Führen Sie die folgenden Schritte aus, um Ihre Einstellung für E-Mail-Benachrichtigungen zu ändern:
1. Greifen Sie mit Ihren eindeutigen Berechtigungsnachweisen für das Konto, das der E-Mail-Adresse zugeordnet ist, die Benachrichtigungen empfängt, auf das Kundenportal zu.
2. Klicken Sie in der Menüleiste auf **Kunde** > **Benutzer** > **Vorgaben für E-Mail**.
3. Wählen Sie in der Liste der Benachrichtigungstypen jeweils die Benachrichtigungen ab, die Sie nicht mehr erhalten wollen.

Ihre Änderungen werden automatisch gespeichert. Diese Einstellungen wirken sich auf die E-Mails aus, die an Sie gesendet werden. Sie haben jedoch keine Auswirkungen auf die E-Mail-Benachrichtigungen anderer Benutzer auf Ihrem Konto.


## Option 'Unterstützung in der EU' festlegen
{: #cp_seteusupported}

Sie können angeben, dass die Unterstützung ausschließlich durch ein Support-Team erfolgen soll, das sich physisch in der Europäischen Union (EU) befindet. Diese Option können Sie auswählen, wenn Sie Ihr Konto einrichten oder ein bestehendes Konto aktualisieren. Führen Sie die folgenden Schritte aus, um die Option **Unterstützung in der EU** festzulegen:
1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Klicken Sie in der Menüleiste auf **Konto** > **Verwalten** > **Unternehmensprofil**.
3. Wählen Sie das Kontrollkästchen **Unterstützung in der EU** aus.
4. Klicken Sie auf **Profilaktualisierung anfordern**.

Falls die Option **Unterstützung in der EU** nicht verfügbar ist, ist möglicherweise für Benutzer in Ihrem Konto der PPTP-VPN-Zugriff aktiviert. Inaktivieren Sie den PPTP-VPN-Zugriff für alle Benutzer in Ihrem Konto, bevor Sie die Option **Unterstützung in der EU** aktivieren. Weitere Informationen zu diesem Thema finden Sie in [PPTP-VPN-Zugriff aktivieren oder inaktivieren](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn).

Weitere Informationen zum Implementieren der Option **Unterstützung in der EU** beim Öffnen eines Support-Tickets enthält der Abschnitt [Support für Ressourcen in der Europäischen Union anfordern](/docs/get-support/howtogetsupport.html#eusupported).
