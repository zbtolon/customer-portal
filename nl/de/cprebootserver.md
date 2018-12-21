---

copyright:

  years: 1994, 2018

lastupdated: "2017-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Server neu starten
{: #customerportal_rebootserver}

Manchmal treten Ereignisse in der {{site.data.keyword.BluSoftlayer_notm}}-Infrastruktur auf, die den Neustart Ihres Servers erfordern.
{:shortdesc}

Führen Sie die folgenden Schritte aus, um Ihren Server erneut zu starten: 
1. Klicken Sie im Kundenportal auf die Registerkarte **Support**.
2. Klicken Sie auf **Neu starten**.
3. Wählen Sie den Server für den Neustart aus und klicken Sie auf **Neu starten**.
4. Wählen Sie eine der folgenden Methoden aus, um den Server erneut zu starten: 
  * Standard (versuchen Sie den Neustart mit IPMI und anschließend mit der Verteilerleiste)
  * IPMI
  * Power Strip
5. Klicken Sie auf **Neu starten**.

Diese Seite bietet auch die Möglichkeit, den Boot im Rescue-Kernel durchzuführen. Dies ist besonders nützlich, wenn ein Problem vorliegt, bei dem der Server aufgrund eines Konfigurationsproblems nicht über das Betriebssystem gebootet werden kann. Nach dem Boot im Rescue-Kernel können Sie das bzw. die Laufwerk(e) Ihres Servers anhängen und dann das Konfigurationsproblem korrigieren. Nachdem das Problem gelöst wurde, können Sie einen Neustart des Servers über die Befehlszeile durchführen und der Server wird in seinem Standardkernel neu gestartet. Nachdem Sie den Befehl zum Neustart abgesetzt haben, wird in der Anzeige die geschätzte Zeit bis zum Abschluss ausgegeben.
