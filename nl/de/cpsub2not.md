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


# Benachrichtigungen abonnieren
{: #cp_bpnotifications}

Manchmal kommt es in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur zu Ereignissen, die eine Aktion erforderlich machen. Einige dieser Ereignisse treten unerwartet auf, andere sind geplante Wartungsaktivitäten, die zur Aufrechterhaltung einer hohen Leistungsfähigkeit der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur erforderlich sind. Kunden werden von diesen Ereignissen weitestmöglich isoliert; bisweilen ist es jedoch nötig, Geräte in den Offlinemodus zu versetzen. Unabhängig von der Auswirkung auf die Kunden ist es hierbei immer erforderlich, transparent, zeitgerecht und informativ vorzugehen.
{:shortdesc}

Damit Sie bei der Nutzung der Cloud keine unangenehmen Überraschungen erleben, müssen Sie rechtzeitig über Wartungsaktivitäten informiert werden. Um diese Informationen zu erhalten, können Sie im Kundenportal Benachrichtigungen abonnieren. Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur nutzt den Benachrichtigungsprozess von EMS (Event Management System, Ereignismanagementsystem) für die folgenden Typen von wichtigen Betriebsereignissen:
* Ungeplante infrastrukturelle Probleme: Derartige Probleme könnten unter bestimmten Umständen für bestimmte Kunden eine Betriebsunterbrechung verursachen.
* Geplante Servicewartung: Dies sind Wartungsaktivitäten, die zur Aufrechterhaltung eines optimalen Status für den Infrastrukturbetrieb erforderlich sind.
* Geöffnete Support-Tickets: Dies sind Alerts, die von Benutzern mit einem Abonnement für Tickets in ihrem Konto geöffnet wurden.

Die Benachrichtigungen der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur sind für Cloudumgebungen konzipiert und beachten daher die folgenden Grundprinzipien:
* Automatisierung über das Kundenportal
* Skalierbarkeit zur Berücksichtigung einer umfangreichen und wachsenden Community
* Aktivierte Zielgruppenspezifik für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur, damit nur die vom Ereignis betroffenen Kunden und Ressourcenuntergruppen ermittelt werden

Damit das Benachrichtigungssystem seine volle Wirksamkeit erzielen kann, müssen Sie den Prozess abonnieren. Falls Sie eine kritische Umgebung nutzen, richten Sie außerdem eine 24-Stunden-Abdeckung ein, wenn dies für Ihre Umgebung erforderlich ist.

Eine Übersicht über die Art der Bereitstellung von Benachrichtigungen in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur enthält der Beitrag [Improving communications for customer-affecting planned events ![Symbol für externen Link](../icons/launch-glyph.svg)](http://blog.softlayer.com/2014/improving-communications-customer-affecting-planned-events){:new_window}.

## Ablaufsteuerungsrichtlinie für Benachrichtigungen
{: #cp_bpgsnotiftimpol}

Der Zeitraum, den die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur den Benutzern vor einem anstehenden Ereignis einräumt, variiert abhängig davon, ob es sich bei dem Ereignis um ein ungeplantes infrastrukturelles Problem oder um eine planmäßige bzw. terminierte Wartung handelt. Generell gibt die Richtlinie für die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur vor, dass Probleme so schnell wie möglich gelöst werden müssen, um das Risiko einer Entstehung weiterer Probleme mit einer größeren Auswirkung zu verhindern oder zu begrenzen. Dies bedeutet, dass selbst planmäßige Wartungen bisweilen mit einer nur kurzfristigen Vorabbenachrichtigung durchgeführt werden.

### Richtlinien im Überblick
{: #cp_bpgsnotifpolover}

Sie werden bei den folgenden Typen von Betriebsunterbrechungen oder Problemen benachrichtigt, die in den einzelnen Abschnitten beschrieben sind.

#### Ungeplante Probleme oder Betriebsunterbrechungen
Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur versorgt betroffene Kunden so schnell wie möglich mit Informationen über Infrastrukturbereich, Ausweichlösungen oder geschätzte Zeit für die Problemlösung, sobald diese Informationen vorliegen. Die rechtzeitige Kommunikation versorgt Sie mit den Informationen, die Sie zur Kontingentplanung benötigen, und sichert zu, dass die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur das Problem behandelt.

#### Planmäßige Wartung
Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur gibt Benachrichtigungen über planmäßige Wartungen im Vorfeld des Ereignisses aus. Es gibt Situationen, in denen die Wartung der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur aufgrund eines Notfalls stattfindet, was zu einer kurzfristigeren Benachrichtigung führen kann. Ziel ist hierbei immer ein optimaler Kompromiss zwischen einer rechtzeitigen Benachrichtigung, die Ihnen Zeit für die Kontingentplanung gibt, und einem Upgrade oder einer Erweiterung der Infrastruktur, die in der Regel zu Verbesserungen bei der Gesamtstabilität oder zu Erweiterungen durch benötigte Funktionalität führt.

#### Sicherheitslücken
Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur isoliert den betroffenen Bereich, erstellt ein Patch, um die Sicherheitslücke zu schließen, und testet den Patch, um sicherzustellen, dass keine verbundenen Funktionen beeinträchtigt werden. Diese Arbeiten erfolgen häufig in Kooperation mit einem anderen Anbieter, der Komponenten der betroffenen Technologie beschaffen könnte. Normalerweise gibt es eine öffentliche Benachrichtigungssperre für Sicherheitspatches, die zum Schutz der Öffentlichkeit kurz gehalten wird, jedoch eine kurzfristigere Vorabbenachrichtigung erforderlich macht. Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur implementiert die Patches in der betroffenen Infrastruktur, bevor die Öffentlichkeit über das Problem informiert wird, da andernfalls das Risiko erhöht würde. Je schneller eine Sicherheitslücke geschlossen wird, desto früher wird das Risiko beseitigt; dies bringt mit sich, dass Sicherheitsprobleme ein kurzes Benachrichtigungsfenster erfordern.

Eines der häufigsten Ziele von Sicherheitsverletzungen ist Software für virtuelle Infrastrukturen. Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur nutzt gängige Open-Source- und Partnertechnologie, um ihr Angebot für virtuelle Server bereitzustellen. Damit ein Sicherheitsfix implementiert werden kann, müssen möglicherweise Kundenserver, auf denen Software für virtuelle Infrastrukturen ausgeführt wird, für die Korrektur offline gesetzt werden und die Umgebung muss neu gestartet werden, was zu einer Betriebsunterbrechung führt. Um die Auswirkungen für die Kunden zu minimieren, hat die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur kürzlich eine Erweiterung des Benachrichtigungsprozesses für virtuelle Infrastrukturen implementiert und die Kommunikation verbessert. Kunden werden mit einer bestimmten Startzeit und einem 90-minütigen Fenster für jeden Pod benachrichtigt, was eine kürzere Unterbrechungsdauer und ein genaueres Timing bewirkt und Ihnen somit eine bessere Vorbereitung ermöglicht. Das Benachrichtigungssystem isoliert die Wartung für jedes Konto, was es der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur ermöglicht, Kunden nach dem Service für ihre jeweiligen Hosts umgehend zu benachrichtigen, meistens deutlich vor Ablauf des 90-minütigen Fensters.

#### Mehrere betroffene Pods oder Rechenzentren
Die {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur bemüht sich um längerfristige Vorankündigungen, sofern die Implementierung des Fixes nicht extrem dringlich ist, um eine noch größere Folgewirkung zu vermeiden.


## Abonnenten zu Ereignisbenachrichtigungen hinzufügen
{: #cp_bpaddsub2eventnotcp}

Immer mehr IBM Kunden nutzen die Services der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur (IaaS), entweder durch vertragliche Vereinbarungen mit IBM über Services für verwaltete Infrastrukturen, durch vertragliche Vereinbarungen über Cloud-Services, die in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur ausgeführt werden, oder durch Direktverträge für Services der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur. Wenn Cloud-Services Infrastruktur einbeziehen, sind nur Benutzer mit einem SoftLayer-Konto zum Empfang von Benachrichtigungen berechtigt (siehe oben). In manchen Fällen möchten Sie jedoch nicht, dass die IBM Teams für Konten oder verwaltete Services, die am Betrieb oder am Support von Infrastrukturservices beteiligt sind, auf Ihre SoftLayer-Konten zugreifen können. Das Kundenportal der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur wurde mit einer neuen Funktion ausgestattet, mit der Sie eine Liste von Abonnenten angeben können (z. B. IBM Mitarbeiter), die Benachrichtigungen empfangen, ohne Berechtigungen für Ihre Konten zu besitzen.

Um eine Liste von Abonnenten anzugeben, können sich Masterbenutzer bei ihrem Kundenportalkonto anmelden und anschließend die folgenden Schritte ausführen:
1. Klicken Sie im Menü **Konto** > **Verwalten** > **Abonnements**.
2. Wählen Sie den Ereignistyp aus, zu dem Sie Abonnenten hinzufügen wollen.
2. Fügen Sie im Popup-Fenster die E-Mail-Adresse(n) hinzu. E-Mail-Adressen können Adressen von IBM oder nicht von IBM sein.
3. Klicken Sie auf **Erstellen**.

E-Mail-Adressen, die als zusätzliche Abonnenten hinzugefügt wurden, empfangen Benachrichtigungen über geplante und ungeplante Ereignisse sowie über geöffnete Support-Tickets. Die Benachrichtigungen enthalten technische Details, was Sie beim Hinzufügen von Abonnenten berücksichtigen sollten. Aufgrund des differenzierten technischen Inhalts der Benachrichtigungen richten sie sich an Abonnenten, die in der Lage sind, die Auswirkung der Benachrichtigung auf Ihre {{site.data.keyword.BluSoftlayer_notm}}-Infrastrukturumgebung im Detail zu verstehen. Das Festlegen von Empfängern als Abonnenten, die die möglichen Auswirkungen für Clients aufgrund der Details in der Benachrichtigung nicht nachvollziehen können, ist kontraproduktiv und somit nicht zu empfehlen.
