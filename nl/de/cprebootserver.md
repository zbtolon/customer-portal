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

# Server neu starten
{: #customerportal_rebootserver}

Manchmal kommt es in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur zu Ereignissen, die einen Warmstart Ihres Servers erforderlich machen.
{:shortdesc}

Führen Sie die folgenden Schritte aus, um Ihren Server neu zu starten:
1. Klicken Sie im Kundenportal auf die Registerkarte **Support**.
2. Klicken Sie auf **Warmstart**.
3. Wählen Sie den Server aus, der neu gestartet werden soll, und klicken Sie auf **Warmstart**.
4. Wählen Sie eine der folgenden Methoden für den Warmstart des Servers aus:
  * Standard (Warmstartversuch zunächst mit PMI und dann mit Power Strip)
  * IPMI
  * Power Strip
5. Klicken Sie auf 'Warmstart'.

Diese Seite bietet auch die Möglichkeit, den Boot im Rescue-Kernel durchzuführen. Dies ist besonders nützlich, wenn ein Problem vorliegt, bei dem der Server aufgrund eines Konfigurationsproblems nicht über das Betriebssystem gebootet werden kann. Nach dem Boot im Rescue-Kernel können Sie das bzw. die Laufwerk(e) Ihres Servers anhängen und dann das Konfigurationsproblem korrigieren. Nachdem das Problem gelöst wurde, können Sie einen Warmstart des Servers über die Befehlszeile durchführen und der Server wird in seinem Standardkernel neu gestartet. Nachdem Sie den Warmstartbefehl abgesetzt haben, wird in der Anzeige die geschätzte Zeit bis zum Abschluss ausgegeben.
