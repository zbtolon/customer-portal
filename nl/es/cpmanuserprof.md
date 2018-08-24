---

copyright:

  years: 1994, 2018

lastupdated: "2018-08-13"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestión de un perfil de usuario
{: #customerportal_accuserprof}

En el portal de clientes, el perfil de usuario incluye varios datos, entre ellos la información de contacto y la clave de API. También es la ubicación en la que se almacenan las contraseñas. Si tiene acceso administrativo, puede cambiar los permisos y el acceso de dispositivo del perfil.
{:shortdesc}

En el perfil de usuario, puede gestionar la información de contacto y las contraseñas, ver claves de API y actualizar permisos y acceso de dispositivo en función de sus permisos.

## Edición de un perfil de usuario
{: #cp_edituserprofile}

Después de crear un perfil de usuario en el portal de clientes, puede editarlo en cualquier momento. Los detalles asociados con el perfil de usuario incluyen información personal, valores de inicio de sesión, detalles de acceso a la API, suscripciones de notificación de usuario y preguntas de seguridad. Utilice los pasos siguientes para editar un perfil de usuario.

1. Acceda al portal de clientes utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse el nombre de usuario para acceder al perfil de usuario asociado para dicho usuario.
4. Edite los detalles del **Perfil de usuario** como sea necesario. Para los usuarios de las cuentas que utilizan IBMid para la autenticación, actualice su correo electrónico y contraseña en su perfil de IBMid. Para obtener más información, consulte la Tabla 1.
5. Si desea restablecer la contraseña después de iniciar la sesión, pulse **Restablecer contraseña** para generar un correo electrónico con detalles sobre cómo cambiar la contraseña.
6. Pulse **Editar usuario** para enviar los cambios.

| Campo | Definición |
|-----|----------|
| Nombre, Apellido | Nombre y apellido del usuario asociado con el perfil de usuario.|
| Dirección de correo electrónico | Dirección de correo electrónico preferido para recibir notificaciones de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Cambiar la dirección de correo electrónico cambia el registro en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Este cambio no afecta al enlace con las credenciales de autenticación de IBMid. Debe cambiar la dirección de correo electrónico para el IBMid desde el perfil de IBMid.|
| Huso horario | Huso horario preferido a utilizar al visualizar datos con indicación de hora.|
| Teléfono, teléfono alternativo| Números de teléfono de contacto preferidos para que los utilice la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.|
| Dirección, Ciudad, País, Estado / provincia, Código postal | Dirección de contacto completa para que la utilice la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.|
{: caption="Tabla 1. Valores de configuración de la información personal para editar un perfil de usuario" caption-side="top"}

|Campo|Definición|
|-----|----------|
| Restringir acceso a IP | Restringir el acceso a una dirección IP cuando se realice un intento por utilizar el portal de clientes en el perfil de usuario asociado. |
| Caducidad de la contraseña en (solo para los usuarios de cuentas que NO utilicen IBMid para la autenticación) | Cantidad de tiempo que una contraseña está asociada con el perfil de usuario antes de que se deba seleccionar una nueva contraseña. |
| Usuario padre | Cuenta de usuario que se considera el usuario padre del perfil de usuario. El usuario padre predeterminado es el ID de cuenta primario. |
| ¿Necesita preguntas de seguridad? | Marque este recuadro de selección cuando sean necesarias preguntas de seguridad durante el inicio de sesión. Si se marca este recuadro, serán necesarias preguntas de seguridad para el perfil de usuario. |
| Contraseña de VPN | Contraseña que se utilizará para acceder a VPN. Pulse el recuadro de selección **Utilizar contraseña del portal para VPN** para utilizar la contraseña del portal de clientes para acceder a la red de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} mediante VPN. |
{: caption="Tabla 2. Iniciar sesión con valores de configuración para editar un perfil de usuario" caption-side="top"}

|Sección|Campo|Definición|
|-------|-----|----------|
| Información de acceso a la API | IBM Prerequisite Scanner permitido | Direcciones IP que puede autenticar en la API con la clave de API exclusiva asociada con el perfil de usuario |
| Suscripciones a notificaciones de usuario | Facturación | Seleccione **Facturación** para recibir una factura por correo electrónico una vez que se cree. |
| Preguntas de seguridad | Pregunta de seguridad | Al editar el perfil, la pregunta de seguridad que debe responder para iniciar sesión.
| Respuestas de seguridad | Respuesta | Respuesta sensible a las mayúsculas y minúsculas en la pregunta de seguridad aplicable. |
{: caption="Tabla 3. Otros valores de configuración para editar un perfil de usuario" caption-side="top"}
Después de enviar las ediciones a un perfil de usuario, los cambios se aplicarán inmediatamente. Puede cambiar el perfil de usuario de nuevo en cualquier momento repitiendo los pasos anteriores.

Para obtener más información sobre cómo configurar una cuenta de IBMid, consulte [Cambio a IBMid](/docs/account/softlayerlink.html#switching-to-ibmid).

## Edición de los permisos de portal de clientes del usuario
{: #cp_editusercpperm}

El administrador de la cuenta establece los permisos de usuario cuando se añada el usuario. Los permisos de usuario los puede editar un usuario autorizado en cualquier momento. Puede ver su propio perfil de usuario y, si es un usuario administrativo, algunos campos de los perfiles de usuario para los usuarios que añada. Los permisos se dividen en cinco separadores: soporte, dispositivos, red, servicios y cuenta. Puede actualizar los permisos para un usuario a la vez y debe guardar los cambios para que pasen a estar activos.

Efectúe los pasos siguientes para editar los permisos de portal de clientes de un usuario.

1. Acceda al portal de clientes utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse el nombre de usuario del usuario para acceder al perfil de usuario.
4. Pulse el icono **Permisos** para acceder a la ventana Permisos.

  Puede que obtenga un mensaje que indica que los cambios no son en el perfil de usuario. Si no se han realizado cambios en el perfil, pulse para descartar los cambios y acceder a la ventana Permisos.
  {: tip}

5. Seleccione los permisos:
  * Para establecer permisos rápidos, seleccione el conjunto de permisos de la lista **Permisos rápidos**. Después de seleccionar un conjunto de permisos, cada permiso que está asociado con el conjunto se mostrará en texto naranja con una flecha naranja que apunta al recuadro de selección. A continuación, pulse **Establecer permisos** para cada separador.
  * Para establecer permisos individuales, marque o desmarque cada recuadro de selección en los separadores para actualizar los permisos del usuario. Pulse **Seleccionar todos los permisos** o **Deseleccionar todos los permisos** en cualquier separador para seleccionar o desmarcar todos los permisos de una vez.
6. Pulse **Editar permisos del portal** para enviar cambios y actualizar los permisos del usuario.
7. Para restablecer los permisos del usuario a los valores originales en lugar de guardarlos, pulse **Restablecer permisos**. Pulse **Cancelar** para cancelar los cambios y volver a la ventana Usuarios.

Los permisos de usuario se actualizan inmediatamente después de enviar los cambios. Si se otorgan permisos, el usuario puede ver o interactuar con las características seleccionadas. El usuario ya no puede ver ni interactuar con las características seleccionadas si se han retirado permisos. Actualice los permisos de nuevo en cualquier momento repitiendo los pasos anteriores.

## Adición de autenticación externa para un usuario
{: #cp_addextauthuser}

Desde el portal de clientes, puede activar la autenticación externa de dos factores (2FA) para añadir protección al iniciar sesión en el portal. Esta capa extra de seguridad protege la cuenta de acceso no verificado, garantizando que los dispositivos, los datos y la información de cuenta estén protegidos. Para obtener más información, consulte [Configuración de autenticación de dos factores](/docs/customer-portal/cpenable2fa.html#customerportal_2fa).


## Cambio del estado de un usuario
{: #cp_changeuserstat}

Su estado determinará su accesibilidad al portal de clientes. Entre las categorías de estado que puede actualizar en la cuenta se encuentran Activo, Inhabilitado y Solo VPN. El estado puede ser modificado por diversas razones y el estado se puede actualizar en cualquier momento. Entre las categorías de estado del cliente se incluyen aquellas que los usuarios pueden actualizar y aquellas actualizadas automáticamente. Incluyen lo siguiente:
<dl>
<dt>Activo</dt>
<dd>El usuario tiene acceso completo al portal de clientes y a VPN basado en permisos establecidos por el administrador de la cuenta. Este estado se puede seleccionar o modificar manualmente en cualquier momento.</dd>
<dt>Inhabilitado</dt>
<dd>El usuario no tiene acceso a ningún permiso ni suscripción en la cuenta, incluido el portal de clientes y VPN. Si otro usuario de la cuenta establece la categoría de estado en inhabilitado, este estado puede ser seleccionado manualmente o cambiado en cualquier momento.</dd>
<dt>Solo VPN</dt>
<dd>El usuario tiene acceso completo a la conectividad de VPN, en función del conjunto de permisos de usuarios, pero no puede acceder al portal de clientes. Este estado se puede seleccionar o modificar manualmente en cualquier momento.</dd>
<dt>Inactivo</dt>
<dd>El usuario no ha accedido al portal de clientes ni a VPN en los últimos 60 días. El estado está generado por el sistema.</dd>
<dt>cancel_pending</dt>
<dd>Un administrador de la cuenta ha cancelado a este usuario y la cancelación se está procesando en este momento. El estado está generado por el sistema.</dd>
</dl>

Efectúe los pasos siguientes para cambiar el estado de un usuario en el portal de clientes.

1. Acceda al portal de clientes utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Usuarios** en la barra de navegación.
3. Seleccione **Cambiar estado de usuario** en la lista **Acciones**.
4. En la lista **Estado**, seleccione el estado adecuado según las definiciones de la lista anterior.
5. Pulse **Guardar**.

Después de actualizar el estado de un usuario, los cambios en la accesibilidad del portal de clientes se alinean con el nuevo estado.


## Edición del acceso VPN de un usuario
{: #cp_edituservpnaccess}

Cuando se añade un usuario nuevo a una cuenta de portal de clientes, se selecciona el acceso VPN desde diversos métodos de conexión, incluidos SSL, PPTP, o una combinación de ambos. Con el acceso VPN, se puede acceder a la red privada en su totalidad o el acceso a la red se puede limitar a una o varias subredes específicas. Puede gestionar y actualizar el acceso a VPN en cualquier momento desde la ventana Usuarios. Efectúe los pasos siguientes para editar el acceso VPN de un usuario.

1. Acceda al portal de clientes utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Acceso VPN** en la barra de navegación.
3. En la columna **Acceso VPN** para el usuario, pulse el enlace del tipo de acceso VPN actual para visualizar la ventana Acceso VPN.
4. En la lista **Tipo de VPN**, seleccione un método VPN (SSL, PPTP, SSL y PPTP, o ninguno) para asignar el usuario.
5. Indique cómo desea gestionar el **Acceso de subred**:
  * Seleccione **Automático** para gestionar automáticamente el acceso de subred
  * Seleccione **Manual** para gestionar manualmente el acceso de subred y, a continuación, marque el recuadro de selección **Otorgar acceso** para cada subred a la que desea que acceda el usuario. Asegúrese de desmarcar los recuadros de selección para subredes a los que no desea que acceda el usuario.
6. Pulse **Guardar**.

Después de actualizar el acceso VPN de un usuario, sus permisos se actualizarán y la columna Acceso VPN mostrará el método de acceso VPN actualizado, si procede.

### Activación o desactivación del acceso VPN
{: #cp_pptpvpn}

Puede activar PPTP VPN para formar un túnel seguro en la red privada de la infraestructura de {{site.data.keyword.BluSoftlayer_full}} que utiliza el software especializado de cliente que se ejecuta en el escritorio o en el dispositivo dedicado. Puede utilizar PPTP si necesita conectar toda su oficina o si no puede utilizar la solución SSL VPN.

Se le asignará una conexión PPTP con conexiones extra disponibles. Puede solicitar soporte para permitir acceso ilimitado a PPTP, que está disponible sin coste extra. Utilice los pasos siguientes para activar o desactivar el acceso PPTP VPN:

1. Acceda al portal de clientes utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Acceso VPN** desde la barra de menús.
3. En la columna **Acceso VPN** para el usuario, pulse el enlace del tipo de acceso VPN actual para visualizar la ventana Acceso VPN.
4. En la lista **Tipo de VPN**, seleccione un método VPN (SSL, PPTP, SSL y PPTP, o ninguno) para asignar el usuario.


## Selección de notificaciones de correo electrónico
{: #cp_select-email-notifications}

Puede seleccionar las notificaciones de correo electrónico que desea recibir de la infraestructura {{site.data.keyword.BluSoftlayer_notm}} y las que no. De forma predeterminada, recibirá todas las notificaciones de correo electrónico pero no podrá cambiarlas siempre que lo desee. Para cambiar los valores de las notificaciones de correo electrónico, siga los pasos siguientes:
1. Acceda al portal de clientes utilizando las credenciales exclusivas de la cuenta asociada con la dirección de correo electrónico que recibe notificaciones.
2. Pulse **Cuenta** > **Usuarios** > **Preferencias de correo electrónico** en la barra de menús.
3. En la lista de tipos de notificaciones, desmarque las notificaciones que ya no desea recibir.

Los cambios se han guardado de forma automática. Estos valores afectan a los correos electrónicos que se le envían, pero no afectan a las notificaciones de correo electrónico de otros usuarios de su cuenta.


## Establecimiento de la opción Soporte en la UE
{: #cp_seteusupported}

Puede indicar que desea soporte exclusivamente de un equipo de soporte ubicado físicamente en la Unión Europea (UE). Puede seleccionar esta opción al configurar su cuenta o al actualizar la cuenta existente. Para establecer la opción **Soporte en la UE**, siga estos pasos:
1. Acceda al portal de clientes utilizando sus credenciales exclusivas.
2. Pulse **Cuenta** > **Gestionar** > **Perfil de la empresa** desde la barra de menús.
3. Marque el recuadro de selección **Soporte en la UE**.
4. Pulse **Solicitar actualización del perfil**.

Si la opción **Soporte en la UE** no está disponible, podría tener usuarios en su cuenta con el acceso PPTP VPN habilitado. Inhabilite el acceso PPTP VPN para todos los usuarios de su cuenta en primer lugar para poder habilitar la opción **Soporte en la UE**. Para obtener más información, consulte [Activación o desactivación del acceso VPN de PPTP](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn).

Para obtener más información sobre la implementación de la opción **Soporte en la UE** al abrir una incidencia de soporte, consulte [Solicitud de soporte para recursos en la Unión Europea](/docs/get-support/howtogetsupport.html#eusupported).
