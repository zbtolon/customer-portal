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


# Zahlung vornehmen
{: #customerportal_makepayment}

Alle Abrechnungsdetails für die {{site.data.keyword.Bluemix}}-Infrastruktur, von Rechnungen bis zu Zahlungsinformationen, werden im Kundenportal geschützt gespeichert. Falls sich Ihre Zahlungsmethode ändert oder Ihre Kreditkarte storniert wird bzw. abläuft, müssen Sie Ihre Zahlungsinformationen aktualisieren, um Verzugsgebühren zu vermeiden.
{:shortdesc}

## Rechnung anzeigen
{: #cp_viewinvoice}

Im Fenster 'Rechnungen' wird jede Rechnung nach Rechnungsnummer, Datum, Rechnungstyp und verschiedenen monetären Bilanzposten zusammengefasst. Rechnungen können einen der folgenden Typen besitzen:

<dl>
<dt>Neu</dt>
<dd>Die erste Rechnung in einer Reihe von Einzelrechnungen.</dd>
<dt>Wiederholt auftretend</dt>
<dd>Eine Rechnung für wiederkehrende Gebühren, die seit mehr als einem Monat für das Konto anfallen.</dd>
<dt>Einmalige Gebühr</dt>
<dd>Eine einmalige Gebühr für verschiedene Ausgaben, die Überschreitungen enthalten kann.</dd>
<dt>Guthaben</dt>
<dd>Ein Guthaben in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für den Kontostand.</dd>
<dt>Rückerstattung</dt>
<dd>Eine Rückbuchung für eine einmalige oder wiederkehrende Gebühr.</dd>
</dl>

Sie können außerdem eine Rechnungszusammenfassung für das Konto anzeigen; hierzu gehören die folgenden Informationen:
  * Aktueller und erwarteter nächste Kontostand
  * Zahlungsmethode
  * Letztes und nächstes Einzelrechnungsdatum

1. Klicken Sie im Menü **Konto** > **Abrechnung** > **Rechnungen**.
2. Sie können die Rechnung entweder im Kundenportal anzeigen oder herunterladen.

Falls Sie die Rechnung im Kundenportal anzeigen, wird eine Liste mit einzeln aufgeführten Rechnungspositionen für die ausgewählte Rechnung angezeigt. Wenn Sie auf eine Stelle in der Zeile für eine Rechnungsposition klicken, werden zusätzliche Einzelangaben zur Gebühr angezeigt. Falls Sie die Rechnung heruntergeladen haben, können Sie sie entsprechend Ihren Browsereinstellungen anzeigen. Heruntergeladene Rechnungen bieten sowohl eine aufgegliederte Zusammenfassung als auch einzeln aufgeführte Abrechnungsdetails für jede Rechnungsposition.

## Zahlungsmethode hinzufügen
{: #cp_cpmanacctbillpay}

Jedem SoftLayer-Konto muss eine bestehende Kreditkarte zugeordnet sein, die in jedem Monat automatisch mit dem Rechnungsbetrag belastet wird. Diese Informationen müssen stets aktuell sein, um Zahlungsverzögerungen zu vermeiden. Sie können sie jederzeit aktualisieren und somit sicherstellen, dass die Zahlungsinformationen immer korrekt sind. Falls die vorhandenen Kreditkarteninformationen richtig sind, Sie jedoch für den aktuellen Saldo eine andere Zahlungsform verwenden möchten, finden Sie unter [Rechnungspositionen verwalten](/docs/customer-portal/cpmanacctbillpay.html#cp_makeonetimepayment) entsprechende Informationen. Führen Sie die folgenden Schritte aus, um eine Zahlungsmethode für ein Konto im Kundenportal hinzuzufügen.

1. Klicken Sie im Menü **Konto** > **Abrechnung** > **Zahlungsmethode**.
2. Geben Sie die erforderlichen Abrechnungsdetails für die Karte in den Feldern im Abschnitt **Rechnungsadresse** ein.
> **Hinweis:** Wenn Sie auf das Kontrollkästchen **Unternehmensinformationen verwenden** klicken, werden die Felder automatisch mit den Unternehmensinformationen gefüllt, die in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur für das Konto angegeben wurden.
3. Geben Sie in den Feldern im Abschnitt **Zahlungsinformationen** die Kreditkarteninformationen ein.
4. Klicken Sie auf **Kreditkarte hinzufügen**, um die Kreditkarte als Methode für die monatliche Zahlung hinzuzufügen.
5. Optional können Sie durch Auswahl von **Unterstützung in der EU** gewährleisten, dass Ihre Service- und Unterstützungsprobleme durch das in Europa ansässige Support-Team bearbeitet werden.  Weitere Informationen zu dieser Option finden Sie unter [Option für Unterstützung in Europa festlegen](/docs/customer-portal/cpmanuserprof.html#cp_seteusupported).

Nachdem Sie die Zahlungsmethode hinzugefügt haben, wird die Anforderung durch Bearbeiter des SoftLayer-Kundenkontos verarbeitet, um die Gültigkeit der Karte sicherzustellen. Validierte Karten können innerhalb von 24 Stunden für das Konto verwendet werden. Die Statusänderung für die Zahlungsmethode wird per E-Mail an den Ansprechpartner gesendet, der beim Hinzufügen der Zahlungsmethode angegeben wurde.

## Einmalzahlung vornehmen
{: #cp_makeonetimepayment}

Sie können Einmalzahlungen entweder über ein PayPal-Konto oder eine Hauptkreditkarte vornehmen; die Zahlung kann entweder den gesamten Saldo oder einen Teilsaldo betreffen. Details von Einmalzahlungen werden nicht zur künftigen Verwendung gespeichert und führen nicht zu einer Änderung der aktuellen Methoden im Konto für die monatliche Zahlung.

1. Navigieren Sie im Kundenportal zur Seite 'Einmalzahlung vornehmen'.
 * Navigieren Sie im Menü zu **Konto** > **Zahlung vornehmen**.
 * Klicken Sie auf der Seite 'Rechnungen' auf **Kontostand bezahlen**.
2. Geben Sie den Zahlungsbetrag im Feld **Zahlungsbetrag** ein.
3. Falls Sie Ihre Zahlung mit PayPal vornehmen, klicken Sie auf **PayPal** und befolgen Sie die von PayPal ausgegebenen Anweisungen, um die Zahlung abzuschließen. Weitere Aktionen sind nicht erforderlich. Falls Sie Ihre Zahlung mit einer Kreditkarte vornehmen, geben Sie in den entsprechenden Feldern **die Kartennummer, das Ablaufdatum und den Sicherheitscode** ein.
4. Geben Sie die Abrechnungsinformationen in den entsprechenden Feldern des Abschnitts **Rechnungsadresse für Kreditkarte** ein.
5. Optional können Sie durch Auswahl von **Unterstützung in der EU** gewährleisten, dass Ihre Service- und Unterstützungsprobleme durch das in Europa ansässige Support-Team bearbeitet werden.  Weitere Informationen zu dieser Option finden Sie unter [Option für Unterstützung in Europa festlegen](/docs/customer-portal/cpmanuserprof.html#cp_seteusupported).
6. Klicken Sie auf **Mit Kreditkarte zahlen**, um die Zahlung auszulösen.

Nachdem Sie die Zahlung ausgelöst haben, wird die Zahlung verarbeitet. Falls im Zusammenhang mit der Zahlung Probleme auftreten, befolgen Sie die Eingabeaufforderungen in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur bzw. bei PayPal, bis das Problem gelöst ist. Die Zahlung wird verarbeitet. Der Betrag wird angewendet und der aktuelle Kontostand wird aktualisiert.
