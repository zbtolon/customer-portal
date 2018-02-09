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


# Häufig gestellte Fragen (FAQs)
{: #bicpfaq}

Die hier aufgeführten häufig gestellten Fragen beziehen sich auf Probleme bei der Verwaltung von Infrastrukturressourcen.
{:shortdesc}


## Wie kann ich meine Berechtigungsnachweise für das Kundenportal abrufen?
{: #bicp_retcreds}

Falls Sie Ihre erste Bestellung aufgeben oder als Benutzer zu einem Konto hinzugefügt werden und zur Authentifizierung Ihre IBMid verwenden, erhalten Sie eine E-Mail mit einem Link, über den Sie mit Ihrer IBMid einsteigen können. Falls Sie Ihren Benutzernamen oder Ihr Kennwort vergessen haben oder nicht mehr auffinden, rufen Sie Ihr [IBMid-Profil ![Symbol für externen Link](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} auf und führen Sie für Ihr Kennwort anhand der Anweisungen, die nach dem Anmeldeprozess ausgegeben werden, eine Zurücksetzung oder Wiederherstellung durch. Sie werden zur Eingabe bestimmter Informationen aufgefordert, wozu auch die Beantwortung  Ihrer Sicherheitsfragen gehören kann.

Wenn Sie Ihre erste Bestellung aufgeben oder als Benutzer zu einem Konto des [Kundenportals ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} hinzugefügt werden und zur Authentifizierung KEINE IBMid verwenden, empfangen Sie eine E-Mail, die Ihren Benutzernamen sowie ein Anfangskennwort enthält, mit dem Sie die Verwendung des Kundenportals beginnen können. Denken Sie daran, Ihr Kennwort nach der ersten Anmeldung zu ändern, indem Sie Ihr [Benutzerprofil bearbeiten](edit-user-profile.html).

Falls Sie Ihr Kennwort nach der Anmeldung vergessen haben, verwenden Sie die Funktion **Kennwort vergessen**, die in der Anmeldeanzeige für das [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} verfügbar ist. Sie werden zur Eingabe bestimmter Informationen aufgefordert, zu denen auch Antworten auf eine Reihe von Sicherheitsfragen gehören, die Sie beim [Bearbeiten Ihres Benutzerprofils](edit-user-profile.html) eingegeben haben.

Falls Sie Ihren Benutzernamen vergessen haben, wenden Sie sich an Ihren Kontoadministrator oder Masterbenutzer, der Ihren Benutzernamen abrufen kann. Als Administrator oder Masterbenutzer für das Konto [wenden Sie sich an den Support](support.html), wenn Sie zusätzliche Unterstützung benötigen.


## Was ist die IBMid und welche Bedeutung hat sie für Benutzer der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur?
{: #bicp_whatisibmid}

Neue Konten müssen zur Authentifizierung die IBMid verwenden. Bestehende Konten verwenden weiterhin den SoftLayer-Benutzernamen und das zugehörige Kennwort für die Authentifizierung, bis durch die Ausführung des Migrationstools zu einer IBMid gewechselt wird. Für Ihr SoftLayer-Konto gibt es einen Masterbenutzer, der berechtigt ist, weitere Benutzer in diesem Konto hinzuzufügen. Weitere Informationen enthält der Abschnitt [Verwaltung von SoftLayer-Konten im Kundenportal](/docs/customer-portal/cphowacctsman.html).

## Wie verknüpfe ich ein bestehendes SoftLayer-Konto?
{: #bicp_linkbmxacct}

Als Masterbenutzer des SoftLayer-Kontos melden Sie sich beim Kundenportal an und klicken Sie im Header auf **Konto verknüpfen**. Weitere Informationen finden Sie unter [IBMid-Benutzerkonten verknüpfen](/docs/admin/softlayerlink.html#link_user_accounts).

## Muss ich bestehender {{site.data.keyword.Bluemix_notm}}-Benutzer sein, damit ich Konten verknüpfen kann?
{: #bicp_bmxusertolink}

Nein. Sie können ein neues {{site.data.keyword.Bluemix_notm}}-Konto erstellen oder ein bestehendes Testkonto bzw. nutzungsabhängiges Konto für {{site.data.keyword.Bluemix_notm}} verknüpfen.


## Wie funktioniert meine Zwei-Faktor-Authentifizierung?
{: #bicp_2fa}

Auf der Kontoebene gibt es keine Auswirkung auf die Konfiguration der Zwei-Faktor-Authentifizierung. Die Zwei-Faktor-Authentifizierung erfolgt nicht für die IBMid, sondern weiterhin kontogebunden. Wenn eine IBMid vielen Konten zugeordnet ist und Sie zwischen Konten wechseln, müssen Sie Ihre Identität bei jedem Wechsel zu einem anderen Konto bestätigen, das eine Zwei-Faktor-Authentifizierung erforderlich macht. Dies gilt sogar dann, wenn das vorherige Konto und das neue Konto beide mit demselben 2FA-Verfahren konfiguriert sind.

Weitere Informationen zur IBMid im Zusammenhang mit der Zwei-Faktor-Authentifizierung finden Sie unter [Zwei-Faktor-Authentifizierung bei verknüpften Konten](/docs/admin/softlayerlink.html#2fa).


## Wer kann Konten verknüpfen?
{: #bicp_wholinkaccts}

Nur Masterbenutzer der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur können SoftLayer- und {{site.data.keyword.Bluemix_notm}}-Konten verknüpfen. Dem primären Eigner des verknüpften {{site.data.keyword.Bluemix_notm}}-Kontos muss außerdem die E-Mail-Adresse eines Masterbenutzers zugeordnet sein.


## Was verwende ich zur Anmeldung bei den einzelnen Portalen?
{: #bicp_logineachport}

Ihre Kontoabrechnung ist verknüpft; Sie können einfach zwischen Ihren SoftLayer- und {{site.data.keyword.Bluemix_notm}}-Konten wechseln, aber die Kontoidentitäten bleiben separat.

* Falls Ihr Konto keine IBMid für die Authentifizierung verwendet, nutzen Sie weiterhin Ihre SoftLayer-ID für SoftLayer-Produkte und -Services sowie Ihre IBMid für {{site.data.keyword.Bluemix_notm}}-Produkte und -Services.

* Falls Ihr Konto eine IBMid für die Authentifizierung verwendet, nutzen Sie Ihre IBMid für den Zugriff sowohl auf Ihr SoftLayer- als auch auf Ihr {{site.data.keyword.Bluemix_notm}}-Konto.


## Warum empfange ich einen Fehler, wenn ich versuche, mich mit meinem SoftLayer-Benutzernamen anzumelden?
{: #bicp_SLloginerror}

Wenn Sie zu einer IBMid gewechselt haben und sich beim Kundenportal mit Ihrem Benutzernamen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur anzumelden versuchen, wird der der Fehler *'Es wurden falsche Anmeldeberechtigungsnachweise angegeben'* angezeigt. Dies liegt daran, dass Sie sich nach dem Wechsel zu einer IBMid nicht mehr mit Ihrem Benutzernamen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur beim Kundenportal anmelden können. Sie müssen im Dialogfeld 'Kontoanmeldung' auf **Mit IBMid anmelden** klicken.

## Warum empfange ich einen Fehler, wenn ich versuche, mich mit meiner IBMid anzumelden?
{: #bicp_IBMidloginerror}

Wenn Sie bei der Anmeldung mit Ihrer IBMid den Fehler *' Diese IBMid oder E-Mail wurde nicht erkannt'* empfangen, vergewissern Sie sich, dass Sie eine vollständig qualifizierte E-Mail-Adresse eingeben. Denken Sie außerdem daran, nicht Ihren Benutzernamen für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur zu verwenden.


##  Ich besitze ein neues SoftLayer-Konto, das die IBMid für die Authentifizierung verwendet. Kann ich dieselbe ID für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur und für {{site.data.keyword.Bluemix_notm}} verwenden?
{: #bicp_loginIBMidSLBlusame}

Ja. Sie können dieselbe IBMid zur Anmeldung bei der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur und bei {{site.data.keyword.Bluemix_notm}} nutzen.


## Ich habe ein {{site.data.keyword.Bluemix_notm}}-Konto verknüpft. Wie ermögliche ich den anderen Mitgliedern meines Teams für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur den Zugriff?
{: #bicp_linkgiveteamaccess}

Sie müssen sie zu {{site.data.keyword.Bluemix_notm}} einladen. Wählen Sie in der {{site.data.keyword.Bluemix_notm}}-Benutzerschnittstelle die Optionen **Konto und Unterstützung** > **Konto** > **Teammitglieder einladen** aus. Nachdem Sie eine Ressourcengruppe ausgewählt haben, wird die Option für das Hinzufügen von Teammitgliedern für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur angezeigt. Möglicherweise müssen Sie sich bei der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur anmelden, damit Sie Einladungen versenden können. {{site.data.keyword.Bluemix_notm}} ruft die Liste der {{site.data.keyword.BluSoftlayer_notm}}-Infrastrukturbenutzer ab; anschließend können Sie auswählen, welche Benutzer für das {{site.data.keyword.Bluemix_notm}}-Konto eingeladen werden sollen.


## Wo finde ich die E-Mail, über die ich den Wechsel zur IBMid abschließen kann?
{: #bicp_ibmidswitchemail}

Falls Sie den Assistenten für den Wechsel zur IBMid durchgearbeitet und die E-Mail noch nicht empfangen haben, kann es mehrere Minuten oder sogar Stunden dauern, bis die E-Mail mit Ihrem Registrierungscode gesendet wird. Sie können zur Seite **Benutzerprofil bearbeiten** im Kundenportal zurückkehren und auf **E-Mail erneut senden** klicken, um den Versuch zu wiederholen.


## Besitze ich uneingeschränkten Rootzugriff auf mein Konto?
{: #bicp_fullrootaccaccess}

Masterbenutzer sowie Personen mit Administratorberechtigungen besitzen im Kundenportal und über die API uneingeschränkten Rootzugriff auf Konten. Die Zugriffsmöglichkeit von Benutzern ohne Administratorberechtigungen wird durch Benutzer mit Verwaltungsrollen gesteuert. Diese Berechtigungen können jederzeit durch eine [Bearbeitung des Benutzerprofils](edit-user-profile.html) im Kundenportal geändert werden.


## Kann ich ein {{site.data.keyword.Bluemix_notm}}-Abonnementkonto verknüpfen?
{: #bicp_linkbmxsubacct}

Alle verknüpften Konten in {{site.data.keyword.Bluemix_notm}} müssen nutzungsabhängige Konten sein. Sie können ein neues nutzungsabhängiges Konto erstellen oder ein bestehendes nutzungsabhängiges Konto verknüpfen. Alternativ können Sie auch ein bestehendes Testkonto verknüpfen; für dieses Konto wird dann jedoch ein Upgrade auf ein nutzungsabhängiges Konto durchgeführt.


## Wie kann ich die Verknüpfung meines {{site.data.keyword.Bluemix_notm}}-Kontos mit meinem {{site.data.keyword.BluSoftlayer_notm}}-Infrastrukturkonto aufheben?
{: #bicp_unlinkacct}

Nachdem Konten verknüpft worden sind, kann die Verknüpfung nicht mehr aufgehoben werden.


## Was ist mein Unternehmensprofil und wo finde ich es?
{: #bicp_whatfindcompprof}

Beim Unternehmensprofil handelt es sich um die Informationen, die bei der Erstellung des Kontos übergeben wurden und die einen Hauptansprechpartner für Ihr Unternehmen sowie Name, Adresse und Telefonnummer des Unternehmens enthalten. Diese Informationen werden zu vielen verschiedenen Zwecken verwendet und sollten jederzeit auf dem neuesten Stand sein. Wenn Sie das Unternehmensprofil für Ihr Konto anzeigen oder Änderungen anfordern wollen, finden Sie im Abschnitt [Unternehmensprofil aktualisieren](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch) weiterführende Informationen.

## Wo finde ich meine Kennwörter für Geräte und Software?
{: #bicp_devswpw}

Geräte- und Softwarekennwörter werden im [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} an zwei Stellen gespeichert. Informationen zum Abrufen von Geräteberechtigungsnachweisen (inklusive Name und Kennwort des Root- oder Adminstratorbenutzers für {{site.data.keyword.baremetal_short}} und {{site.data.keyword.virtualmachinesshort}}) finden Sie unter [Mit Geräten in der Snapshotansicht interagieren](/docs/vsi/vsi_interact_device_snapshot_view.html). Softwareberechtigungsnachweise, die mithilfe des Kundenportals manuell aufgezeichnet werden, können Sie anhand der Angaben im Abschnitt [Gerätezugriff verwalten](/docs/vsi_device_access.html) ohne großen Aufwand anzeigen und abrufen.

##Wie sorge ich dafür, dass meine Webdaten synchron bleiben?
{: #bicp_webdatasync}

Für die Erhaltung der Datenkonsistenz zwischen realen Servern sind Sie zwar selbst verantwortlich, aber {{site.data.keyword.BluSoftlayer_full}} bietet ein privates Netz, das Sie ohne Nutzungsgebühren für die Synchronisierung verwenden können.


## Was ist das Ereignismanagementsystem?
{: #bicp_whatisems}

Das Ereignismanagementsystem (Event Management System, EMS) ist ein Toolset, mit dem die gemeinsame Nutzung von Informationen durch {{site.data.keyword.BluSoftlayer_full}} und Benutzer über ungeplante infrastrukturelle Probleme und anstehende planmäßige Wartungsereignisse optimiert wird. Hierzu werden zielgruppenspezifische und abonnementbasierte E-Mail-Alerts für diese Vorfälle verwendet, die eine gemeinsame Nutzung des aufgetretenen Ereignistyps ermöglichen. Das EMS stellt Benutzern mit einem Abonnement zusätzliche Details über die Gesamtauswirkung des Ereignisses sowie einen aktuellen Status für das gegenwärtig bearbeitete ungeplante Ereignis (Unplanned Incident in Progress, UIP) zur Verfügung.

## Wie und an welcher Stelle kann ich ein Gerät stornieren?
{: #bicp_candev}

Sie können ein Gerät jederzeit über das [Kundenportal ![Symbol für externen Link](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} stornieren. Weitere Informationen zur Ausführung einer Stornierungsanforderung finden Sie unter [Gerät stornieren](/vsi/vsi_managing.html).
