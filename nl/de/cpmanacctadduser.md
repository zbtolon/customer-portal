---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-05"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Benutzer zu einem SoftLayer-Konto hinzufügen
{: #customerportal_addusertocpacct}

Mit den Produkten und Services, die einem Konto zugeordnet sind, können einer oder mehrere Benutzer interagieren. Als Masterbenutzer können Sie jederzeit Benutzer hinzufügen.
{:shortdesc}

Falls Sie {{site.data.keyword.BluSoftlayer_full}}-Infrastrukturbenutzer verwalten, ist es von dem Zugriff, der Ihrem Benutzerkonto zugeordnet ist, sowie von der Konfiguration Ihres Kontos abhängig, welche SoftLayer-Konten Sie verwalten können. Falls Sie der Masterbenutzer sind oder als Kontoeigner Verwaltungszugriff besitzen, können Sie andere Kundenportalbenutzer verwalten. Falls Ihr Konto nicht als Masterbenutzer konfiguriert ist, können Sie Ihr Benutzerprofil verwalten.

Abhängig von Ihrem Zugriff können Sie entweder Ihr eigenes SoftLayer-Konto oder die Konten der anderen Benutzer im Fenster 'Benutzer' verwalten. Im Fenster 'Benutzer' im [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} werden Benutzer angezeigt, denen ein Konto zugeordnet ist. Die im Fenster 'Benutzer' verfügbaren Interaktionen variieren abhängig davon, wie Ihre eindeutige Kontoberechtigung festgelegt ist.
  * Als Masterbenutzer des Kontos können Sie alle Benutzer anzeigen, die dem Konto zugeordnet sind.

  Falls Sie die Masteranmeldeberechtigungsnachweise für Ihr Konto gemeinsam nutzen müssen, gehen Sie hierbei umsichtig vor. Ihre Masteranmeldung steuert alle Aspekte Ihres Kontos und sollte geschützt sein. Um anderen Benutzern die Verwendung des Kundenportals zu ermöglichen, konfigurieren Sie einzelne oder berechtigungsbasierte Benutzer. Auf diese Weise haben Sie die größte Kontrolle darüber, wer mit bestimmten Aspekten Ihres Kontos interagieren kann.
  {:tip}
  * Falls Sie Verwaltungszugriff besitzen, können Sie alle Benutzer anzeigen, die Sie erstellt haben, sowie alle von diesen Benutzern erstellten Benutzer, sofern Sie diese Benutzer zum Verwalten anderer Benutzer berechtigt haben. Außerdem können Sie Aktionen für jeden Benutzer ausführen, der dem Konto zugeordnet ist, was das Bearbeiten des Zugriffs auf das Kundenportal, das Ändern des Benutzerstatus und das Entfernen von Benutzern einschließt.
  * Falls Sie nicht der Masterbenutzer des Kontos sind und keinen Verwaltungszugriff besitzen, wird lediglich Ihr Profil angezeigt. Sie können mit Ihrem eigenen Konto interagieren, beispielsweise den API-Schlüssel anzeigen, den VPN-Zugriff bearbeiten und eine externe Authentifizierung hinzufügen.

Informationen zur Verwaltung von Benutzern über die {{site.data.keyword.Bluemix_notm}}-Konsole enthalten die Abschnitte [Eigenes Konto verwalten](/docs/admin/adminpublic.html#signing-up-for-ibm-cloud) und [Identität und Zugriff verwalten](/docs/iam/quickstart.html#getstarted). Zusätzliche Angaben über die {{site.data.keyword.Bluemix_notm}}-Konsole finden Sie unter [Funktionsweise der {{site.data.keyword.Bluemix_notm}}-Konsole](/docs/overview/ui.html#ui).

Unterschiedliche Personen in einer Organisation besitzen verschiedene Rollen und Zuständigkeiten; Benutzerberechtigungen können somit nicht universell für jeden Benutzer passend festgelegt werden. Daher können Sie Benutzer zum Kundenportal mit Rollen hinzufügen, damit sichergestellt ist, dass jede Person bzw. Gruppe ausschließlich Zugriff auf die für sie zulässigen Elemente besitzt. Falls irrtümlicherweise Änderungen vorgenommen oder Berechtigungen widerrufen wurden, können Sie dies bis zum Benutzer oder zur Gruppe zurückverfolgen und auf diese Weise sicherstellen, dass Sie eine passende Schulung anbieten oder Benutzerberechtigungen aktualisieren können. Dies verringert viele Risiken und erlaubt es den Benutzern, sich auf ihre angegebene Rolle im Kundenportal zu konzentrieren.

Führen Sie zum Hinzufügen eines Benutzers zu einem Konto die folgenden Schritte aus.

1. Greifen Sie unter Verwendung Ihrer eindeutigen Berechtigungsnachweise auf das Kundenportal zu.
2. Wählen Sie in der Navigationsleiste die Optionen **Konto > Benutzer** aus.
3. Klicken Sie auf **Benutzer hinzufügen**.
4. Füllen Sie die erforderlichen Felder im Abschnitt **Persönliche Informationen** aus, inklusive des Status, eines Benutzernamens und der E-Mail-Adresse für die Kommunikation und Benachrichtigungen des Kundenportals, wozu auch die anfängliche Benachrichtigung über das Festlegen eines Kennworts für das Konto gehört.

  Optional können Sie auch auf das Kontrollkästchen **Standardunternehmensinformationen verwenden** klicken, um die Firmenadresse auszufüllen, statt die Adresse für den Benutzer einzugeben.
  {: tip}

5. Füllen Sie die erforderlichen Felder im Abschnitt **Einstellungen für Anmeldung** aus, wozu auch die Angabe gehört, ob die Einstellungen vom Benutzer bearbeitet werden können, ob die IP-Adresse eingeschränkt ist und ob der Benutzer Sicherheitsfragen definieren und verwenden muss oder nicht. Außerdem können Sie für alle Benutzer, die keine IBMid verwenden, den Zeitraum angeben, nach dem das Kennwort abläuft.
**Hinweise:**
* Falls Sie die IBMid für die Authentifizierung verwenden, aktualisieren Sie die Kennwörter in Ihren [IBMid-Profilen ![Symbol für externen Link](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window}, indem Sie die Anweisungen unter **Anmelden** befolgen.
* Klicken Sie auf das Kontrollkästchen **Benutzerportalkennwort für VPN**, um das Kundenportalkennwort und das VPN-Kennwort zu synchronisieren.
6. Klicken Sie auf **Benutzer hinzufügen**.

Nachdem Sie ein Konto für einen Benutzer erstellt haben, empfängt der Benutzer eine E-Mail-Benachrichtigung, damit er die Einrichtung seines Kontos durch das Festlegen eines Kennworts sowie optional durch das Definieren von Sicherheitsfragen abschließt, sofern Sie angegeben haben, dass Sicherheitsfragen erforderlich sind.

Wie sich Benutzer ohne den Verwaltungszugriff eines Masterbenutzers beim Kundenportal anmelden, ist von dem Masterbenutzer abhängig, der den Benutzerzugriff in den zugehörigen SoftLayer-Konten bereitgestellt hat:
  * Falls der Masterbenutzer eine IBMid für die Authentifizierung besitzt, hat jeder vom Masterbenutzer erstellte Benutzer eine IBMid.
  * Falls der Masterbenutzer eine {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur-ID für die Authentifizierung besitzt, hat jeder vom Masterbenutzer erstellte Benutzer einen {{site.data.keyword.BluSoftlayer_notm}}-Infrastrukturbenutzernamen. Der Masterbenutzer und jeder von ihm erstellte Benutzer muss das Migrationstool ausführen, um auf eine IBMid zu wechseln.
  * Falls keiner der obigen Fälle zutrifft (beispielsweise bei einem IBM Business Partner), teilt Ihnen der Support mit, welche Benutzer-ID zu verwenden ist.

## Benutzerberechtigungen für das Konto festlegen
{: #cp_setuserpermsacct}

Führen Sie zum Festlegen der Berechtigungen für einen gerade hinzugefügten Benutzer die folgenden Schritte aus.

1. Klicken Sie auf das Symbol **Berechtigungen**, das als Benutzerbild mit einem Schloss dargestellt ist.
2. Aktualisieren Sie die **Benutzerberechtigungen** auf allen Registerkarten für den neuen Benutzer.
> **Hinweis:** Wählen Sie eine Option in der Liste **Schnellberechtigungen** aus, um empfohlene Berechtigungssets für drei Benutzertypen anzuzeigen. Klicken Sie auf **Berechtigung festlegen**, um das empfohlene Berechtigungsset auszuwählen, oder passen Sie die Zugriffsmöglichkeit des Benutzers durch Auswahl einzelner Optionen auf jeder verfügbaren Registerkarte an.
3. Klicken Sie auf **Portalberechtigungen hinzufügen**, um die Berechtigungen hinzuzufügen, oder klicken Sie auf **Berechtigungen zurücksetzen**, um die Berechtigungen für den Benutzer zurückzusetzen.
4. Klicken Sie auf das Symbol **Gerätezugriff**, auf dem drei Server dargestellt sind.
5. Klicken Sie auf das Kontrollkästchen für jedes Gerät, auf das der Benutzer zugreifen können soll.
6. Klicken Sie nach Auswahl der Geräte auf **Gerätezugriff aktualisieren**.

Sie empfangen daraufhin eine E-Mail mit Links und Informationen, die Sie durch die Einrichtung einer IBMid für die Authentifizierung bei diesem Konto führen. Diese Schritte können die Erstellung einer neuen IBMid umfassen, falls das Konto eine IBMid für die Authentifizierung verwendet. Die Einladung läuft nach 7 Tagen ab. Sie können jedoch Ihren Administrator bitten, die Einladung erneut zu senden.

Bei allen anderen Authentifizierungsfällen kann sich der Benutzer jederzeit beim Kundenportal anmelden, nachdem er hinzugefügt wurde, und mit den verschiedenen, dem Konto zugeordneten Produkten und Services arbeiten. Sie können einen Benutzer jederzeit inaktivieren.
