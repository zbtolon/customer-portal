---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-28"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}


# Häufig gestellte Fragen (FAQs)
{: #bicpfaq}

## Wie kann ich meine Berechtigungsnachweise für das Kundenportal abrufen?
{: #bicp_retcreds}
{: faq}

Falls Sie Ihre erste Bestellung aufgeben oder als Benutzer zu einem Konto hinzugefügt werden und zur Authentifizierung Ihre IBMid verwenden, erhalten Sie eine E-Mail mit einem Link, über den Sie mit Ihrer IBMid einsteigen können. Falls Sie Ihren Benutzernamen oder Ihr Kennwort vergessen haben oder nicht mehr auffinden, rufen Sie Ihr [IBMid-Profil ![Symbol für externen Link](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} auf und führen Sie für Ihr Kennwort eine Zurücksetzung oder Wiederherstellung durch. Sie werden zur Eingabe bestimmter Informationen aufgefordert, wozu auch die Beantwortung Ihrer Sicherheitsfragen gehören kann.

Wenn Sie Ihre erste Bestellung aufgeben oder als Benutzer zu einem Konto des [Kundenportals ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} hinzugefügt werden und zur Authentifizierung keine IBMid verwenden, empfangen Sie eine E-Mail, die Ihren Benutzernamen sowie ein Anfangskennwort enthält, mit dem Sie die Verwendung des Kundenportals beginnen können. Denken Sie daran, Ihr Kennwort nach der ersten Anmeldung zu ändern, indem Sie Ihr Benutzerprofil bearbeiten.

Falls Sie Ihr Kennwort nach der Anmeldung vergessen haben, verwenden Sie die Funktion **Kennwort vergessen**, die in der Anmeldeanzeige für das Kundenportal verfügbar ist. Sie werden zur Eingabe bestimmter Informationen aufgefordert, zu denen auch Antworten auf eine Reihe von Sicherheitsfragen gehören, die Sie beim Einrichten Ihres Benutzerprofils angegeben haben.

Falls Sie Ihren Benutzernamen vergessen haben, wenden Sie sich an Ihren Kontoadministrator oder Masterbenutzer, der Ihren Benutzernamen abrufen kann. Als Administrator oder Masterbenutzer des Kontos wenden Sie sich an den Support, wenn Sie zusätzliche Unterstützung benötigen.

## Was ist die IBMid?
{: #bicp_whatisibmid}
{: faq}

Neue Konten müssen zur Authentifizierung die IBMid verwenden. Bestehende Konten verwenden weiterhin den SoftLayer-Benutzernamen und das zugehörige Kennwort für die Authentifizierung, bis durch die Ausführung des Migrationstools zu einer IBMid gewechselt wird. Für Ihr SoftLayer-Konto gibt es einen Masterbenutzer, der berechtigt ist, weitere Benutzer in diesem Konto hinzuzufügen. 

## Wie verknüpfe ich ein bestehendes SoftLayer-Konto?
{: #bicp_linkbmxacct}
{: faq}

Als Masterbenutzer des SoftLayer-Kontos melden Sie sich beim Kundenportal an und klicken Sie im Header auf **Konto verknüpfen**. Weitere Informationen finden Sie unter [IBMid-Benutzerkonten verknüpfen](/docs/account/softlayerlink.html).

## Muss ich bestehender {{site.data.keyword.Bluemix_notm}}-Benutzer sein, damit ich Konten verknüpfen kann?
{: #bicp_bmxusertolink}
{: faq}

Nein. Sie können ein neues {{site.data.keyword.Bluemix_notm}}-Konto erstellen oder ein bestehendes {{site.data.keyword.Bluemix_notm}}-Lite-Konto bzw. nutzungsabhängiges Konto für {{site.data.keyword.Bluemix_notm}} verknüpfen.

## Wie funktioniert die Zwei-Faktor-Authentifizierung?
{: #bicp_2fa}
{: faq}

Auf der Kontoebene gibt es keine Auswirkung auf die Konfiguration der Zwei-Faktor-Authentifizierung (2FA). 2FA erfolgt nicht pro IBMid, sondern weiterhin pro Konto. Wenn eine IBMid vielen Konten zugeordnet ist und Sie zwischen den Konten wechseln, müssen Sie Ihre Identität bei jedem Wechsel zu einem anderen Konto bestätigen, für das eine Zwei-Faktor-Authentifizierung erforderlich ist. Dies gilt sogar dann, wenn das vorherige Konto und das neue Konto beide mit demselben 2FA-Verfahren konfiguriert sind.

Weitere Informationen zur IBMid im Zusammenhang mit der Zwei-Faktor-Authentifizierung finden Sie unter [Mehrfaktorauthentifizierung bei verknüpften Konten](/docs/account/softlayerlink.html#2fa).

## Wer kann Konten verknüpfen?
{: #bicp_wholinkaccts}
{: faq}

Nur Masterbenutzer der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur können SoftLayer- und {{site.data.keyword.Bluemix_notm}}-Konten verknüpfen. Dem primären Eigner des verknüpften {{site.data.keyword.Bluemix_notm}}-Kontos muss außerdem die E-Mail-Adresse eines Masterbenutzers zugeordnet sein.

## Was verwende ich zur Anmeldung bei den einzelnen Konsolen?
{: #bicp_logineachport}
{: faq}

Ihre Kontoabrechnung ist verknüpft; Sie können einfach zwischen Ihren SoftLayer- und {{site.data.keyword.Bluemix_notm}}-Konten wechseln, aber die Kontoidentitäten bleiben separat.

* Falls Ihr Konto keine IBMid für die Authentifizierung verwendet, nutzen Sie weiterhin Ihre SoftLayer-ID für SoftLayer-Produkte und -Services sowie Ihre IBMid für {{site.data.keyword.Bluemix_notm}}-Produkte und -Services.

* Falls Ihr Konto eine IBMid für die Authentifizierung verwendet, nutzen Sie Ihre IBMid für den Zugriff sowohl auf Ihr SoftLayer- als auch auf Ihr {{site.data.keyword.Bluemix_notm}}-Konto.

## Warum erhalte ich beim Versuch, mich mit meinem SoftLayer-Benutzernamen anzumelden, eine Fehlernachricht?
{: #bicp_SLloginerror}
{: faq}

Wenn Sie zu einer IBMid gewechselt haben und sich beim Kundenportal mit Ihrem Benutzernamen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur anzumelden versuchen, wird der Fehler 'Es wurden falsche Anmeldeberechtigungsnachweise angegeben' angezeigt. Nach dem Wechsel zu einer IBMid können Sie sich nicht mehr mit Ihrem Benutzernamen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur beim Kundenportal anmelden. Sie müssen im Dialogfeld 'Kontoanmeldung' auf **Mit IBMid anmelden** klicken.

## Warum erhalte ich beim Versuch, mich mit meiner IBMid anzumelden, eine Fehlernachricht?
{: #bicp_IBMidloginerror}
{: faq}

Bei der Anmeldung mit Ihrer IBMid wird der Fehler ' Diese IBMid oder E-Mail wurde nicht erkannt' angezeigt. Stellen Sie sicher, dass Sie eine vollständig qualifizierte E-Mail-Adresse eingeben. Denken Sie außerdem daran, nicht Ihren Benutzernamen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur zu verwenden.

## Können Teammitglieder der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur auf mein verknüpftes Konto zugreifen?
{: #bicp_linkgiveteamaccess}
{: faq}

Sie müssen sie zu {{site.data.keyword.Bluemix_notm}} einladen. Klicken Sie in der {{site.data.keyword.Bluemix_notm}}-Konsole auf **Verwalten** > **Konto** > **Benutzer**. Nach Auswahl einer Ressourcengruppe können Sie Teammitglieder der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur hinzufügen. Sie müssen sich möglicherweise beim Kundenportal anmelden, bevor Sie Einladungen versenden können. {{site.data.keyword.Bluemix_notm}} ruft die Liste der {{site.data.keyword.BluSoftlayer_notm}}-Infrastrukturbenutzer ab; anschließend können Sie auswählen, welche Benutzer für das {{site.data.keyword.Bluemix_notm}}-Konto eingeladen werden sollen.

## Wo finde ich die E-Mail, über die ich den Wechsel zur IBMid abschließen kann?
{: #bicp_ibmidswitchemail}
{: faq}

Falls Sie den Assistenten für den Wechsel zur IBMid durchgearbeitet und die E-Mail noch nicht empfangen haben, kann es mehrere Minuten oder sogar Stunden dauern, bis die E-Mail mit Ihrem Registrierungscode an Sie gesendet wird. Sie können zur Seite **Benutzerprofil bearbeiten** im Kundenportal zurückkehren und auf **E-Mail erneut senden** klicken, um den Versuch zu wiederholen.

## Besitze ich uneingeschränkten Rootzugriff auf mein Konto?
{: #bicp_fullrootaccaccess}
{: faq}

Masterbenutzer sowie Personen mit Administratorberechtigungen besitzen im Kundenportal und über die API uneingeschränkten Rootzugriff auf Konten. Die Zugriffsmöglichkeit von Benutzern ohne Administratorberechtigungen wird durch Benutzer mit Verwaltungsrollen gesteuert. Diese Berechtigungen können von Administratoren im Kundenportal aktualisiert werden, indem sie ein [Benutzerprofil bearbeiten](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Ohne Administratorberechtigungen können Sie Ihr Benutzerprofil im Kundenportal bearbeiten, indem Sie oben in der Anzeige auf Ihren Benutzernamen klicken.

## Kann ich ein {{site.data.keyword.Bluemix_notm}}-Abonnementkonto verknüpfen?
{: #bicp_linkbmxsubacct}
{: faq}

Alle verknüpften Konten in {{site.data.keyword.Bluemix_notm}} müssen Lite-Konten oder nutzungsabhängige Konten sein. 

## Wie kann ich die Verknüpfung meines Kontos aufheben?
{: #bicp_unlinkacct}
{: faq}

Nachdem Konten verknüpft worden sind, kann die Verknüpfung nicht mehr aufgehoben werden.


## Was ist mein Unternehmensprofil und wo finde ich es?
{: #bicp_whatfindcompprof}
{: faq}

Beim Unternehmensprofil handelt es sich um die Informationen, die beim Erstellen des Kontos übergeben wurden und die einen Hauptansprechpartner für Ihr Unternehmen sowie Name, Adresse und Telefonnummer des Unternehmens enthalten. Diese Informationen werden zu vielen verschiedenen Zwecken verwendet und sollten jederzeit auf dem neuesten Stand sein. Wenn Sie das Unternehmensprofil für Ihr Konto anzeigen oder Änderungen anfordern wollen, finden Sie im Abschnitt [Unternehmensprofil aktualisieren](/docs/customer-portal/cpmanacctcompprofcont.html#cp_updcompprof) weiterführende Informationen.

## Wo finde ich meine Kennwörter für Geräte und Software?
{: #bicp_devswpw}
{: faq}

Geräte- und Softwarekennwörter werden im Kundenportal an zwei Stellen gespeichert. Informationen zum Abrufen von Geräteberechtigungsnachweisen (inklusive Name und Kennwort des Root- oder Administratorbenutzers für {{site.data.keyword.baremetal_short}} und {{site.data.keyword.virtualmachinesshort}}) finden Sie unter [Mit Geräten in der Snapshotansicht interagieren](/docs/vsi/vsi_interact_device_snapshot_view.html). Softwareberechtigungsnachweise, die mithilfe des Kundenportals manuell aufgezeichnet werden, können Sie anhand der Angaben im Abschnitt [Gerätezugriff verwalten](/docs/vsi/vsi_device_access.html) ohne großen Aufwand anzeigen und abrufen.

## Wie sorge ich dafür, dass meine Webdaten synchron bleiben?
{: #bicp_webdatasync}
{: faq}

Für die Erhaltung der Datenkonsistenz zwischen realen Servern sind Sie zwar selbst verantwortlich, aber {{site.data.keyword.BluSoftlayer_full}} bietet ein privates Netz, das Sie ohne Nutzungsgebühren für die Synchronisierung verwenden können.

## Was ist das Ereignismanagementsystem?
{: #bicp_whatisems}
{: faq}

Das Ereignismanagementsystem (Event Management System, EMS) ist ein Toolset, mit dem die gemeinsame Nutzung von Informationen durch {{site.data.keyword.BluSoftlayer_full}} und Benutzer über ungeplante infrastrukturelle Probleme und anstehende planmäßige Wartungsereignisse optimiert wird. Hierzu werden zielgruppenspezifische und abonnementbasierte E-Mail-Alerts für diese Vorfälle verwendet, die eine gemeinsame Nutzung des aufgetretenen Ereignistyps ermöglichen. Das EMS stellt Benutzern mit einem Abonnement Details über die Gesamtauswirkung des Ereignisses sowie einen aktuellen Status für das gegenwärtig bearbeitete ungeplante Ereignis (Unplanned Incident in Progress, UIP) zur Verfügung.

## Kann ich ein Gerät stornieren?
{: #bicp_candev}
{: faq}

Sie können ein Gerät jederzeit im Kundenportal stornieren. Weitere Informationen zur Ausführung einer Stornierungsanforderung finden Sie unter [Gerät stornieren](/docs/vsi/vsi_managing.html).
