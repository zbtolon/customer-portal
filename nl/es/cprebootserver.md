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

# Reinicio del servidor
{: #customerportal_rebootserver}

A veces, los sucesos se producen en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} que requiere que reinicie el servidor.
{:shortdesc}

Efectúe los pasos siguientes para reiniciar el servidor:
1. Desde el portal de clientes, pulse el separador **Soporte**.
2. Pulse **reiniciar**.
3. Seleccione el servidor que desea reiniciar y pulse **Reiniciar**.
4. Seleccione uno de los métodos siguientes para reiniciar el servidor:
  * Valor predeterminado (intento de reinicio con IPMI y luego con el multiplicador)
  * IPMI
  * Multiplicador
5. Pulse **reiniciar**.

Esta página también ofrece la posibilidad de arrancar en el kernel de rescate, lo cual es muy útil si tiene problemas en los que el servidor no se puede arrancar en el SO debido a un problema de configuración. Después de arrancar en el kernel de rescate, puede montar la unidad, o las unidades, del servidor y, a continuación, solucionar el problema de configuración. Tras solucionar el problema, puede reiniciar el servidor desde la línea de mandatos y el servidor se reiniciará en el kernel predeterminado para su servidor. Una vez que haya emitido el mandato de reinicio, verá un tiempo estimado de finalización.
