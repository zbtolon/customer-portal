---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Suscripción a notificaciones
{: #cp_bpnotifications}

A veces, se producen sucesos en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} que necesitan acción; algunos son inesperados y otros son actividades de mantenimiento planeadas necesarias para mantener la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} operativa y en su condición pico. Los clientes están aislados de estos sucesos tanto como es posible, pero a veces es necesario poner al equipo fuera de línea. Independientemente del impacto para los clientes, siempre es necesario ser transparente, oportuno e informativo.
{:shortdesc}

Puesto que debe controlar su experiencia en la nube, necesita información oportuna sobre las actividades de mantenimiento. Para obtener esta información, puede suscribirse a notificaciones desde el portal de clientes. La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} utiliza el proceso de notificación de Event Management System (EMS) para los siguientes tipos de sucesos operativos importantes:
* Problemas de infraestructura no planificados: Problemas que podrían causar una interrupción en determinadas condiciones para clientes específicos
* Mantenimiento de servicio planificado: Mantenimiento necesario para que la infraestructura siga funcionando en estado óptimo
* Incidencias de soporte abiertas: Alertas suscritas por los usuarios de incidencias abiertas en su cuenta

Las notificaciones de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} se han diseñado para los entornos de nube adhiriéndose a los siguientes principios fundamentales:
* Automatizadas a través del portal de clientes
* Escalables para alcanzar a una comunidad grande y en crecimiento
* Destinadas habilitando la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para identificar solo a los clientes y al subconjunto de recursos afectados por el suceso.

Para que el sistema de notificación sea totalmente efectivo, suscríbase al proceso. Si tiene un entorno crítico que lo requiera, establezca también la cobertura de 24 horas.

Para obtener una visión general de cómo se proporcionan las notificaciones de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}, consulte [Mejora de comunicaciones para los sucesos planificados que afectan a los clientes ![Icono de enlace externo](../icons/launch-glyph.svg)](http://blog.softlayer.com/2014/improving-communications-customer-affecting-planned-events){:new_window}.

## Política de tiempo de notificación
{: #cp_bpgsnotiftimpol}

El periodo de tiempo que la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} da a los usuarios antes de un suceso pendiente difiere, dependiendo de si el suceso es un problema de infraestructura no planeado o un mantenimiento previsto o planificado. Generalmente, la política de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} es remediar problemas lo antes posible para eliminar o minimizar el riesgo de más problemas al desarrollar lo que podría tener un mayor impacto. Esto significa que a veces incluso el mantenimiento planificado se realiza con solo una notificación brevemente avanzada.

### Visión general de políticas
{: #cp_bpgsnotifpolover}

Se le notificará de los siguientes tipos de paradas o problemas como se describe en cada sección.

#### Problemas o paradas no planificados
La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} se comunica con los clientes afectados lo antes posible con información sobre el alcance de la infraestructura, las soluciones o las estimaciones de resolución tan pronto como se conozca esa información. La comunicación puntual le ofrece la información que necesita para planificar contingencias y proporciona la garantía de que la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} está tratando el problema.

#### Mantenimiento planificado
La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} proporciona notificación para el mantenimiento planificado con antelación a los sucesos. Hay momentos en que el mantenimiento de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} es una emergencia, lo que podría dar lugar a una notificación avanzada con menos tiempo. El objetivo es siempre encontrar el equilibrio ideal entre dar una cantidad razonable de avisos avanzados para permitirle planificar contingencias y actualizar o ampliar la infraestructura que normalmente da lugar a mejoras en la estabilidad global o a la adición de prestaciones necesarias.

#### Vulnerabilidades de la seguridad
La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} aísla la zona afectada, crea un parche para cerrar la vulnerabilidad, y prueba el parche para asegurarse de que no esté afectada ninguna función colateral. A menudo, este trabajo se realiza con otro proveedor que podría suministrar partes de la tecnología afectada. Normalmente hay un embargo de notificaciones públicas para los parches de seguridad, que se conservan abreviadas para proteger al público, pero esto necesita un periodo de notificación avanzada más corto. La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} implementa los parches en la infraestructura afectada antes de que se dé noticia al público del problema, lo que de lo contrario podría aumentar el riesgo. Cuanto más rápido se cierre la vulnerabilidad, antes se eliminará el riesgo, lo que significa que los problemas de seguridad necesitan una ventana de notificación breve.

Uno de los objetivos más frecuentes para las infracciones de seguridad es el software de infraestructura virtual. La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} utiliza tecnología de código abierto y de socios popular para entregar su oferta de Servidor virtual. Para implementar un arreglo de seguridad, los servidores de los clientes que ejecutan software de infraestructura virtual pueden tener que ponerse fuera de línea para aplicar un parche y rearrancar el entorno, provocando interrupciones. Para minimizar el impacto a los clientes, la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} ha implementado recientemente una mejora en el proceso de notificaciones para la infraestructura virtual: Comunicaciones mejoradas. Se notifica a los clientes con una hora de inicio específica y una ventana de 90 minutos para cada pod, lo que da lugar a un tiempo de interrupción más breve y un tiempo más preciso para ayudarle a prepararse mejor. El sistema de notificación aísla el mantenimiento a cada cuenta, lo que permite a la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} notificar a los clientes tan pronto como se dé servicio a sus hosts específicos, lo que ocurre con más frecuencia mucho antes de la ventana de 90 minutos.

#### Varios POD o centros de datos afectados
La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} se esfuerza por dar un aviso más avanzado, a menos que haya una urgencia extrema por implementar el arreglo para evitar un impacto secundario aún mayor.


## Adición de suscriptores a notificaciones de sucesos
{: #cp_bpaddsub2eventnotcp}

Cada vez más, los clientes de IBM se basan en los servicios de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} (IaaS), ya sea mediante la contratación con IBM para servicios de infraestructura gestionados, la contratación de servicios en la nube que se ejecutan en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} o la contratación directa con los servicios de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Cuando los servicios en la nube implican la infraestructura, solo estarán autorizados para recibir notificaciones los usuarios de la cuenta de SoftLayer, tal como se describe en la sección anterior. En algunos casos, es posible que no desee que los equipos de IBM Account o de Managed Service implicados en las operaciones o el soporte de los servicios de infraestructura accedan a sus cuentas de SoftLayer. Se ha añadido una nueva característica al portal de clientes de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}, lo que le permite designar una lista de suscriptores, por ejemplo personal de IBM, para que reciba notificaciones sin tener privilegios en las cuentas.

Para designar una lista de suscriptores, los usuarios maestro pueden iniciar sesión en su cuenta de portal de clientes y seguir estos pasos:
1. Pulse **Cuenta** > **Gestionar** > **Suscripciones** en el menú.
2. Elija el tipo de suceso al que añadir a los suscriptores.
2. En la ventana emergente, añada la dirección o direcciones de correo electrónico. Las direcciones de correo electrónico pueden ser de IBM o no.
3. Pulse **Crear**.

Las direcciones de correo electrónico añadidas como suscriptores adicionales reciben notificaciones de sucesos planificados y no planificados, e incidencias de soporte abiertas. Las notificaciones contienen detalles técnicos, así que debe tenerlo en cuenta al añadir suscriptores. Debido a la naturaleza técnica detallada de las notificaciones, los suscriptores deseados son aquellos que puedan entender, detalladamente, cómo afecta la notificación al entorno de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Los destinatarios suscritos que no pueden comprender el impacto de clientes potenciales en función de los detalles de la notificación son contraproducentes y no se recomiendan en absoluto.
