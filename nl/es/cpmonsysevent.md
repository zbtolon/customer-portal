---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# Supervisión de sucesos del sistema de la infraestructura de {{site.data.keyword.Bluemix_notm}}
{: #customerportal_monevent}

Puede supervisar sucesos del sistema para que sus sistemas se sigan ejecutando sin contratiempos. Para obtener información sobre la configuración y la gestión de servidores virtuales en la infraestructura de {{site.data.keyword.BluSoftlayer_full}}, consulte [Iniciación a los servidores virtuales](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers).
{:shortdesc}

## Visualización de un registro de auditoría para una cuenta
{: #cp_viewacctauditlog}

Cada cuenta del portal del cliente viene con un registro de auditoría que realiza el seguimiento de las interacciones de cada usuario en el portal del cliente. Entre las interacciones rastreadas se incluyen intentos de inicio de sesión (correctas e incorrectas), actualizaciones de la velocidad de puerto, encendido o apagado y rearranques, y las interacciones realizadas por el personal de soporte de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Efectúe los pasos siguientes para ver un registro de auditoría para una cuenta de usuario.

1. Acceda al [Portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Gestionar** > **Registro de auditoría** desde la barra de navegación para acceder al registro de auditoría.

El registro de auditoría muestra inicialmente las últimas 25 interacciones realizadas por los usuarios en la cuenta. Puede ver hasta 200 interacciones en cualquier momento. Actualice el número de resultados mostrados desde la lista desplegable **Visualizar**. Si se han modificado los valores, la columna **Acción** para la interacción contendrá un enlace. Pulse cualquier enlace para ver el valor afectado por la acción y los detalles sobre el cambio. Al pulsar el nombre de dispositivo o el nombre de usuario para cualquier interacción, se le redirigirá a la pantalla Detalles de dispositivo o a la pantalla Perfil de usuario, respectivamente.

## Visualización de registros de acceso de un usuario
{: #cp_viewuserlogs}

Los Registros de acceso muestran datos por cada intento de acceso realizado por un usuario del portal del cliente específico. Los registros muestran una indicación de fecha y hora y la dirección IP por cada intento de acceso. Utilice los pasos siguientes para ver los Registros de acceso de un usuario.

1. Acceda al [portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Usuarios** en la barra de menús para acceder a la ventana Usuarios.
3. En la lista desplegable **Acciones**, seleccione **Ver registro de auditoría** para ver el registro de acceso del usuario.

El registro de acceso para cada usuario muestra los intentos de acceso realizados por dicho usuario por fecha, junto con la dirección IP desde la que se ha realizado el intento de acceso. La información del registro de acceso es de solo lectura, por lo que las ediciones en el contenido no se pueden realizar en cualquier momento. Puede ver los registros de acceso de nuevo en cualquier momento repitiendo los pasos anteriores. Para salir de los registros y volver a la pantalla Usuarios, pulse el enlace **Ver todos los usuarios** en la parte superior de la pantalla.
