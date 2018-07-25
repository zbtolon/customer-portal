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

# Rearranque del servidor
{: #customerportal_rebootserver}

A veces, los sucesos se producen en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} que requiere que rearranque el servidor.
{:shortdesc}

Efectúe los pasos siguientes para rearrancar el servidor:
1. Desde el portal de clientes, pulse el separador **Soporte**.
2. Pulse **Rearrancar**.
3. Seleccione el servidor que se rearrancará y pulse **Rearrancar**.
4. Seleccione uno de los métodos siguientes para rearrancar el servidor:
  * Valor predeterminado (intento de rearranque con IPMI y luego con el multiplicador)
  * IPMI
  * Multiplicador
5. Pulse Rearrancar.

Esta página también ofrece la posibilidad de arrancar en el kernel de rescate, lo cual es muy útil si tiene problemas en los que el servidor no se puede arrancar en el SO debido a un problema de configuración. Después de arrancar en el kernel de rescate, puede montar la unidad, o las unidades, del servidor y, a continuación, solucionar el problema de configuración. Tras solucionar el problema, puede rearrancar el servidor desde la línea de mandatos y el servidor se rearrancará en el kernel predeterminado para su servidor. Una vez que haya emitido el mandato de rearranque, verá un tiempo estimado de finalización.
