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


# Supervisión de sucesos del entorno y del sistema
{: #customerportal_cpmonenvsysevent}

La supervisión del entorno significa que tiene la capacidad para comprobar los dispositivos en cualquier momento y que se le notificará automáticamente si se desactiva alguno de sus dispositivos. También puede supervisar sucesos del sistema para que sus sistemas se sigan ejecutando sin contratiempos.  
{: shortdesc}

## Supervisión del entorno
{: #cpmonenv}

Como mínimo, utilice la supervisión de ping básica, pero puede personalizar sus opciones de supervisión de la forma que se ajuste mejor a sus necesidades de negocio.

### Manténgase informado de los sucesos de mantenimiento de red y de los no planeados
{: #cp_stayinfomaintevent}

De vez en cuando, es inevitable tener que llevar a cabo mantenimiento de red de emergencia y programado. La infraestructura de {{site.data.keyword.BluSoftlayer_full}} mantiene muchos canales para mantenerle informado de todos los sucesos de mantenimiento de emergencia y planificados. Además, puede [suscribirse a las notificaciones por correo electrónico](/docs/customer-portal/cpsub2not.html) desde el Event Management System. Este servicio gratuito envía mensajes de correo electrónico automáticamente a los usuarios suscritos sobre sucesos no planeados que pueden afectar a los servicios.

### Utilización de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} móvil
{: #cp_bmxinframobile}

Utilice la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} móvil para gestionar los dispositivos de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} sobre la marcha mediante su dispositivo móvil iOS o Android. La funcionalidad dentro de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} móvil incluye soporte de incidencias, control básico de dispositivos y supervisión del ancho de banda.

La aplicación móvil de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} complementa la funcionalidad del portal de clientes, ya que permite supervisar la información crítica sobre la infraestructura desde cualquier sitio mediante el dispositivo móvil conectado a la red. La aplicación evoluciona rápidamente y se añaden nuevas funciones con regularidad, pero puede utilizar la aplicación móvil para efectuar las tareas siguiente, entre otras:
  * Ver, crear y actualizar incidencias de soporte
  * Supervisar el estado del dispositivo, incluido el ancho de banda y las alarmas
  * Cerrar y reiniciar los servidores nativos y los servidores virtuales
  * Ver facturas de cuentas y realizar pagos únicos
  * Acceder y examinar contenido almacenado en Object Storage

La aplicación móvil de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} está disponible en varias plataformas populares de dispositivo móvil, de forma gratuita en las tiendas de aplicaciones de cada plataforma.

## Supervisión de servidores
{: #customerportal_monservers}

Defina una supervisión para comprobar el estado del servidor y saber así cuándo escalar. Puede utilizar servicios de supervisión estándar o Nimsoft. Puede utilizar la supervisión estándar, o básica, con el método de ping y respuesta mediante el uso de un ping lento o de servicio desde el portal de clientes de {{site.data.keyword.BluSoftlayer_notm}}. También puede utilizar supervisión Nimsoft, o avanzada, desde el portal de clientes o en uno de estos tres niveles: básico, avanzado y premium. Para obtener más información sobre los servidores nativos, específicamente, consulte [Guía de iniciación con servidores nativos](/docs/bare-metal/index.html#getting-started).

## Supervisión de sucesos del sistema
{: #customerportal_monevent}

Puede supervisar sucesos del sistema visualizando registros de auditoría y de acceso.

### Visualización de un registro de auditoría para una cuenta
{: #cp_viewacctauditlog}

Cada cuenta del portal de clientes viene con un registro de auditoría que realiza el seguimiento de las interacciones de cada usuario en el portal de clientes. Se realiza seguimiento, por ejemplo, de las siguientes interacciones:
  * Intentos de inicio de sesión (correctas e incorrectas)
  * Actualizaciones de la velocidad de puerto
  * Encendido o apagado y rearranques
  * Interacciones realizadas por el personal de soporte de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.

Efectúe los pasos siguientes para ver un registro de auditoría para una cuenta de usuario.

1. Acceda al [Portal de clientes ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Gestionar** > **Registro de auditoría** desde la barra de navegación para acceder al registro de auditoría.

El registro de auditoría muestra inicialmente las últimas 25 interacciones realizadas por los usuarios en la cuenta. Puede ver hasta 200 interacciones en cualquier momento. Actualice el número de resultados mostrados desde la lista desplegable **Visualizar**. Si se han modificado los valores, la columna **Acción** para la interacción contendrá un enlace. Pulse cualquier enlace para ver el valor afectado por la acción y los detalles sobre el cambio. Al pulsar el nombre de dispositivo o el nombre de usuario para cualquier interacción, se le redirigirá a la pantalla Detalles de dispositivo o a la pantalla Perfil de usuario.

### Visualización de registros de acceso de un usuario
{: #cp_viewuserlogs}

Los Registros de acceso muestran datos por cada intento de acceso realizado por un usuario del portal de clientes específico. Los registros muestran una indicación de fecha y hora y la dirección IP por cada intento de acceso. Utilice los pasos siguientes para ver los Registros de acceso de un usuario.

1. Acceda al [portal de clientes ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Usuarios** en la barra de menús para acceder a la ventana Usuarios.
3. En la lista desplegable **Acciones**, seleccione **Ver registro de auditoría** para ver el registro de acceso del usuario.

El registro de acceso para cada usuario muestra los intentos de acceso realizados por dicho usuario por fecha, junto con la dirección IP desde la que se ha realizado el intento de acceso. La información del registro de acceso es de solo lectura, por lo que las ediciones en el contenido no se pueden realizar en cualquier momento. Puede ver los registros de acceso de nuevo en cualquier momento repitiendo los pasos anteriores. Para salir de los registros y volver a la pantalla Usuarios, pulse el enlace **Ver todos los usuarios**.
