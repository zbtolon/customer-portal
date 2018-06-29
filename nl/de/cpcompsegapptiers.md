---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Umgebung schützen und skalieren
{: #cp_compsegapptierssecscal}

Zwei der wichtigsten Aspekte, die ein Systemadministrator beim Hosting einer Anwendung berücksichtigen muss, sind die Sicherheit und die Skalierbarkeit der Anwendung.
{:shortdesc}

## Systeme mit Firewalls schützen
{: #cp_bpsecuresystem}

Verwenden Sie die verfügbaren Hardware-Firewalls um sicherzustellen, dass Ihr Gerät jederzeit sicher ist. Sie können Hardware-Firewalls bedarfsgerecht ohne Ausfallzeit bereitstellen, wenn die Regeln ordnungsgemäß festgelegt wurden, um Ihren Server vor unerwünschter Aktivität zu schützen.

Firewalls sind Add-on-Services für Geräte, die Sie manuell konfigurieren und aktivieren müssen, damit sie wirksam sind. Sie können entbehrliche Ports sperren und öffentliche Ports für private netzbasierte Systeme inaktivieren, um die externe Zugänglichkeit zu Ihren Systemen weiter zu verwalten. Regelmäßige Scans auf Sicherheitslücken sorgen dafür, dass alle ausstehenden oder unbekannten Sicherheitsrisiken erkannt werden und Sie Risiken schnell begrenzen können. 

Nach dem Anfordern Ihrer Firewall muss sie aktiviert werden und es müssen Regeln festgelegt werden.

### Firewall aktivieren
{: #cp_bpnofirewalbypass}

Die Anschaffung einer Firewall ist ein guter erster Schritt für den Schutz Ihrer Systeme, aber der bloße Kauf bewirkt nicht, dass Sie geschützt sind. Nachdem Ihre Firewall bereitgestellt wurde, befindet sie sich im **Bypassmodus** ohne festgelegte Regeln. Um Ihre Firewall betriebsbereit zu machen, müssen Sie Regeln erstellen und die Firewall aktivieren, damit sie unerwünschte Aktivitäten blockieren kann.


## Umgebung durch Segmentierung der Anwendungsschichten schützen
{: #cp_copmsecenv}

Wenn Sie Ihre logischen Anwendungsschichten in physische Infrastrukturschichten segmentieren, können Sie mittels Zugriffssteuerungslisten (Access Control Lists, ACLs) eine größere Sicherheit erzielen. Beim Segmentieren Ihrer Anwendungsschichten muss insbesondere der Datenverkehr, den Sie für jede Schicht ermöglichen wollen, und auch sein Ursprung berücksichtigt werden. Hierzu müssen Sie sich Gedanken darüber machen, wie die Anwendung grundlegend funktioniert und welche Services voneinander abhängig sind, um den angeforderten Inhalt für den Benutzer bereitzustellen. 

Ziehen Sie beispielsweise eine zweischichtige Anwendung in Betracht, die sich auf eine Web-Front und ein Datenbank-Back-End stützt. Hier müssen Sie sicherstellen, dass Port 80 und 443 (bei Verwendung von SSL) für das Internet auf Ihren Web-Servern geöffnet sind. In diesem Fall würden Sie wahrscheinlich auch alle Ports für das Internet sperren und Ihre Server über VPN mit dem privaten Netz der {{site.data.keyword.BluSoftlayer_full}}-Infrastruktur verwalten. Sie würden wahrscheinlich auch die Bindung der öffentlichen IP-Adresse auf Ihrem Datenbankserver aufheben und den gesamten Datenverkehr zu diesem Server über Port 1433 (für MSSQL) bzw. Port 3306 (für {{site.data.keyword.mysql}}) aus Ihrem Web-Server abwickeln. Sie können Ihren Datenbankserver genau wie Ihren Web-Server über das private Netz verwalten. Und Sie können auf dem Datenbankserver eine Software-Firewall einrichten, um den gesamten Datenverkehr aus dem Web-Server an die speziellen Datenbankports zu sperren. 

Wenn Sie Ihre Umgebung auf diese Weise einrichten, erhöhen Sie die Sicherheit, indem Sie Personen vom Zugriff auf SSH oder RDP über das Internet abhalten und den gesamten Internetdatenverkehr an Ihre Datenbank inaktivieren. Die Erstellung von ACLs zwischen Ihrer Webschicht und Ihrer Datenbankschicht erschwert eine Gefährdung Ihrer Datenbank, falls Ihr Web-Server beeinträchtigt wird. 

## Umgebung durch Segmentierung der Anwendungsschichten skalieren
{: #cp_copmscaleenv}

Eine mehrschichtige Umgebung vereinfacht im Vergleich zu vertikalen oder Einzelhostarchitekturen ebenfalls die Skalierbarkeit. Sie können eine mehrschichtige Umgebung einrichten, um die Skalierung Ihrer Anwendung zu vereinfachen, indem Sie eine Skalierung für diejenigen Services ermöglichen, die mehr Ressourcen benötigen. Falls beispielsweise im obigen Szenario Ihr Web-Server überfordert ist, können Sie einfach einen weiteren Web-Server bereitstellen. Anschließend können Sie Site- oder Anwendungsdaten replizieren und einen Lastausgleich oder Umlauf-DNS konfigurieren, damit Ihre beiden Web-Server die Webarbeitslast aufteilen können. Umlauf-DNS oder Lastausgleich ermöglichen eine hohe Verfügbarkeit Ihrer Umgebung, da mehrere Web-Server auf eingehende Anforderungen antworten können. Falls ein einzelner Server ausfällt, ist ein weiterer Knoten für die Abwicklung von Benutzeranforderungen verfügbar. 

Auch Ihre Datenbank können Sie horizontal skalieren. Bei einer {{site.data.keyword.mysql}}-Datenbank haben Sie unter anderem die Möglichkeit, einen weiteren physischen Server einzurichten und ihn in einer {{site.data.keyword.mysql}}-Replikation als untergeordnet zu konfigurieren. Sie können alle Datenbankschreibvorgänge für den Master und alle Datenbanklesevorgänge für einen oder mehrere Slaves segmentieren, um die Datenbank für die Unterstützung einer größeren Arbeitslast zu skalieren. Diese Art der Konfiguration trägt zur Hochverfügbarkeit bei, weil Sie einem Slave den Status eines Masters geben können. Anschließend können Sie sowohl den Lese- als auch den Schreibdatenverkehr an den Slave weiterleiten, wenn Ihr {{site.data.keyword.mysql}}-Masterknoten ausfällt. 

Diese Beispiele sind nur einige der vielen Möglichkeiten für den Schutz und die Skalierung Ihrer Umgebung. Falls Sie Fragen oder Probleme hinsichtlich der bestmöglichen Architektur Ihrer Umgebung in Bezug auf Sicherheit oder Skalierbarkeit haben, können Sie sich an das Vertriebsentwicklungsteam der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur wenden. 
