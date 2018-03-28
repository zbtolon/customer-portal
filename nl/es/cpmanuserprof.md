---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-17"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Gestión de un perfil de usuario
{: #customerportal_accuserprof}

En el portal del cliente, un perfil de usuario contiene una serie de datos sobre el usuario, incluida la información de contacto y la clave de API. También es la ubicación en la que se almacenan las contraseñas. Además, si tiene acceso administrativo, puede cambiar los permisos y el acceso de dispositivo del perfil.
{:shortdesc}

En el perfil de usuario, puede gestionar la información de contacto y las contraseñas, ver claves de API y actualizar permisos y acceso de dispositivo adicionales en función de sus permisos.

## Edición de un perfil de usuario
{: #cp_edituserprofile}

Después de crear un perfil de usuario en el portal de cliente, puede editarlo en cualquier momento. Los detalles asociados con el perfil de usuario incluyen información personal, valores de inicio de sesión, detalles de acceso a la API, suscripciones de notificación de usuario y preguntas de seguridad. Utilice los pasos siguientes para editar un perfil de usuario.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse el nombre de usuario para acceder al perfil de usuario asociado para dicho usuario.
4. Edite los detalles del **Perfil de usuario** como sea necesario. Para los usuarios de las cuentas que utilizan IBMid para la autenticación, actualice su correo electrónico y contraseña en su perfil de IBMid. Consulte la Tabla 1 para obtener más información.
5. Si desea restablecer la contraseña después de iniciar la sesión, pulse **Restablecer contraseña** para generar un correo electrónico que le permita cambiar la contraseña.
6. Pulse **Editar usuario** para enviar los cambios.

| Campo | Definición |
|-----|----------|
| Nombre, apellido | Nombre y apellido del usuario asociado con el perfil de usuario.|
| Dirección de correo electrónico | Dirección de correo electrónico preferido para recibir notificaciones de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} relacionada con la cuenta. Cambiar la dirección de correo electrónico cambia el registro en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Este cambio no afecta al enlace con las credenciales de autenticación de IBMid. Debe cambiar la dirección de correo electrónico para el IBMid desde el perfil de IBMid.|
| Huso horario | Huso horario preferido a utilizar al visualizar datos con indicación de hora.|
| Teléfono, teléfono alternativo| Números de teléfono de contacto preferidos para que los utilice la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.|
| Dirección, Ciudad, País, Estado / provincia, Código postal | Dirección de contacto completa para que la utilice la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.|
{: caption="Tabla 1. Valores de configuración de la información personal para editar un perfil de usuario" caption-side="top"}

|Campo|Definición|
|-----|----------|
| Restringir acceso a IP | Dirección IP para restringir el acceso al intentar utilizar el portal del cliente en el perfil de usuario asociado. |
| Caducidad de la contraseña en (solo para los usuarios de cuentas que NO utilicen IBMid para la autenticación) | Cantidad de tiempo que una contraseña debe estar asociada con el perfil de usuario antes de que se deba seleccionar una nueva contraseña. |
| Usuario padre | Cuenta de usuario que se considera el usuario padre del perfil de usuario. El usuario padre predeterminado es el ID de cuenta primario. |
| ¿Necesita preguntas de seguridad? | Seleccione este recuadro de selección cuando deban ser necesarias preguntas de seguridad durante el inicio de sesión. Si se marca este recuadro, serán necesarias preguntas de seguridad para el perfil de usuario. |
| Contraseña de VPN | Contraseña que se utilizará para acceder a VPN. Pulse el recuadro de selección **Utilizar contraseña del portal para VPN** para utilizar la contraseña del portal del cliente para acceder a la red de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} mediante VPN. |
{: caption="Tabla 2. Iniciar sesión con valores de configuración para editar un perfil de usuario" caption-side="top"}

|Sección|Campo|Definición|
|-------|-----|----------|
| Información de acceso a la API | IP permitidas | Direcciones IP permitidas para autenticarse en la API utilizando la clave de API exclusiva asociada con el perfil de usuario |
| Suscripciones a notificaciones de usuario | Facturación | Marque el recuadro de selección **Facturación** para recibir una factura por correo electrónico una vez que se haya creado. |
| Preguntas de seguridad | Pregunta de seguridad | Al editar su perfil, esta es la pregunta que debe responder para iniciar sesión cuando se hayan activado las preguntas de seguridad para su perfil.
| Respuestas de seguridad | Respuesta | Respuesta sensible a las mayúsculas y minúsculas en la pregunta de seguridad aplicable. |
{: caption="Tabla 3. Otros valores de configuración para editar un perfil de usuario" caption-side="top"}
Después de enviar las ediciones a un perfil de usuario, los cambios se aplicarán inmediatamente. Puede cambiar el perfil de usuario de nuevo en cualquier momento repitiendo los pasos anteriores.  

Consulte [Conmutar a IBMid](/docs/account/softlayerlink.html#switching-to-ibmid) para obtener más información sobre la configuración de una cuenta de IBMid.

## Edición de los permisos de portal de cliente del usuario
{: #cp_editusercpperm}

Los permisos de usuario en el portal de cliente los configura el administrador de la cuenta cuando se añade el usuario y un usuario autorizado los puede editar en cualquier momento. Puede ver su propio perfil de usuario y, si es un usuario administrativo, algunos campos de los perfiles de usuario para los usuarios que añada. Los permisos se dividen en cinco separadores: soporte, dispositivos, red, servicios y cuenta. Puede actualizar los permisos para un usuario a la vez y debe guardar los cambios para que pasen a estar activos.

Efectúe los pasos siguientes para editar los permisos de portal de cliente de un usuario.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse el nombre de usuario del usuario para acceder al perfil de usuario.
4. Pulse el icono **Permisos** para acceder a la ventana Permisos.

  Puede que obtenga un mensaje que indica que los cambios no se han guardado en el perfil de usuario. Si no se han realizado cambios en el perfil, pulse para descartar los cambios y acceder a la ventana Permisos.
  {: tip}

5. Seleccione los permisos:
  * Para establecer permisos rápidos, seleccione el conjunto de permisos de la lista **Permisos rápidos**. Después de seleccionar un conjunto de permisos, para permiso asociado con el conjunto se mostrará en texto naranja con una flecha naranja que apunta al recuadro de selección. A continuación, pulse **Establecer permisos** para cada separador.
  * Para establecer permisos individuales, marque o desmarque cada recuadro de selección en los separadores para actualizar los permisos del usuario. Pulse **Seleccionar todos los permisos** o **Deseleccionar todos los permisos** en cualquier separador para seleccionar o deseleccionar todos los permisos de una vez.
6. Pulse **Editar permisos del portal** para enviar cambios y actualizar los permisos del usuario.
7. Para restablecer los permisos del usuario a los valores originales en lugar de guardarlos, pulse **Restablecer permisos**. Pulse **Cancelar** para cancelar los cambios y volver a la ventana Usuarios.

Los permisos de usuario se actualizan inmediatamente después de enviar los cambios. Si se han otorgado permisos, el usuario puede ver o interactuar con las características seleccionadas. Si se han retirado permisos, el usuario ya no puede ver ni interactuar con las características seleccionadas. Los permisos pueden ser actualizados de nuevo en cualquier momento repitiendo los pasos anteriores.

## Adición de autenticación externa para un usuario
{: #cp_addextauthuser}

Desde el portal del cliente, puede activar la autenticación externa de dos factores para añadir protección adicional al iniciar sesión en el portal. Esta capa adicional de seguridad protege la cuenta de acceso no verificado, garantizando que los dispositivos, los datos y la información de cuenta estén protegidos. Esta autenticación externa está disponible en las siguientes formas:

* **Symantec Identify Protection** es la herramienta de autenticación externa más comúnmente utilizada, que proporciona un código de seguridad dinámico que se utiliza además del nombre de usuario y de la contraseña al acceder al portal del cliente.
* La autenticación de **PhoneFactor** proporciona autenticación de usuario fuera de banda desde un teléfono, un SMS, o una app para móvil. PhoneFactor requiere un número de teléfono válido al que debe tener acceso en cualquier momento al intentar autenticarse.

Puede añadir ambos métodos de autenticación externa, por usuario, por una [pequeña tarifa mensual ![Icono de enlace externo](../icons/launch-glyph.svg)](http://www.softlayer.com/services/security/){:new_window}. Utilice los pasos siguientes para añadir autenticación externa para un usuario del portal del cliente.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Seleccione **Añadir autenticación externa** desde la lista **Acciones** para el usuario.
4. Seleccione el tipo de autenticación externa que se pedirá:
  * **Symantec Identity Protection** -- Especifique el ID de credenciales del usuario en el campo **ID de credenciales**.
  * **PhoneFactor** -- Elija un [método de autenticación](#cp_phonefacauthmeths).
5. Pulse **Continuar**.
6. Siga las solicitudes de la ventana para **Código promocional** y **Acuse de recibo de MSA**.
7. Pulse **Pedir autenticación externa** para completar el pedido.

Después de añadir la autenticación externa para un usuario, los pasos siguientes dependen del tipo de autenticación.
* Si Symantec Identity Protection está habilitado, debe añadir el código de seguridad asociado con el ID de credenciales del usuario que se ha especificado en el sistema en el momento de añadir Symantec Identity Protection a la cuenta.
* Si PhoneFactor está habilitado, el usuario debe [activar PhoneFactor](#cp_actphonefacauth) para utilizar este tipo de autenticación de dos factores con la cuenta.

### Activación de la autenticación de PhoneFactor
{: #cp_actphonefacauth}

Después de añadir PhoneFactor, debe activar manualmente la autenticación externa con PhoneFactor a través del portal del cliente. Puesto que PhoneFactor utiliza el contacto manual, es importante asegurarse de que todos los números de teléfono asociados con la cuenta estén actualizados en todo momento. No mantener la información de contacto actualizada podría provocar que no se pueda acceder al portal de cliente ni a VPN cuando PhoneFactor esté activo. Cuando PhoneFactor se haya añadido correctamente, recibirá un correo electrónico para confirmar que se ha añadido PhoneFactor. Tras recibir el correo electrónico, efectúe los pasos siguientes para activar la autenticación de PhoneFactor.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse el nombre de usuario para acceder al perfil de usuario asociado para dicho usuario.
4. Desplácese a la sección **Valores de PhoneFactor**.

  Si la sección Valores de PhoneFactor no está disponible, compruebe en primer lugar que haya recibido el correo electrónico de suministro de PhoneFactor que indica que PhoneFactor se ha suministrado. Si se ha suministrado PhoneFactor y la sección no está disponible, cree una incidencia de soporte. Si PhoneFactor no se ha suministrado aún, espere el correo electrónico e inténtelo de nuevo. Si PhoneFactor aún no se ha añadido, consulte [adición de la autenticación externa para un usuario](/docs/customer-portal/cpmanuserprof.html#cp_addextauthuser).
  {: tip}

5. Seleccione **Activo** en la lista **Estado**.
6. Edite el **Número de teléfono principal** para la autenticación.
  1. Pulse el enlace **Editar**.
  2. Escriba el **Código de país**, el **Número de teléfono** y la **Extensión**, si es aplicable, en los campos asociados.
  3. Pulse **Autenticar y guardar número** para completar la autenticación.

    Al añadir un número de teléfono para la autenticación, debe estar junto al teléfono. Después de pulsar **Autenticar**, se llamará al número y se le solicitará que realice un paso para autenticar el número. Los números de teléfono no se pueden autenticar sin haber completado estos pasos.
    {: tip}

  4. Para añadir un **Número de teléfono secundario**, repita estos pasos.
7. Seleccione el **Método de contacto** en la lista **Método**.
8. Seleccione un **Tipo de PIN** en la lista **Tipo de PIN**.
9. Si selecciona **Una vez** > **Valor de PIN**, escriba el PIN en el campo **Valor de PIN**.
10. Pulse **Actualizar** para actualizar los cambios y activar la autenticación de PhoneFactor.

Después de activar PhoneFactor, el portal de cliente o VPN necesita la autenticación a través de PhoneFactor. Después de autenticarse con las credenciales de usuario, un mensaje le indicará que se ha intentado dicha autenticación de PhoneFactor. Usted, o el usuario que está añadiendo, debe estar cerca del teléfono listado con PhoneFactor para completar la autenticación. PhoneFactor intentará autenticarse cinco veces. Tras cinco intentos de autenticación infructuosos, se le bloqueará durante aproximadamente una hora. Usted, o un usuario con acceso administrativo a la cuenta, puede cambiar los valores de autenticación de PhoneFactor en cualquier momento.  Usted, o un administrador de la cuenta, puede desactivar PhoneFactor en cualquier momento.

#### Métodos de autenticación de PhoneFactor
{: #cp_phonefacauthmeths}

Si configura PhoneFactor como el tipo de autenticación, podrá elegir una de las siguientes opciones como método de autenticación:
<dl>
<dt>Llamada de teléfono y estándar (sin pin)</dt>
<dd>Con esta opción habilitada, cuando inicie la sesión en el portal, recibirá una llamada de teléfono en el número principal habilitado. Cuando responda a la llamada, se le indicará que pulse la tecla # para completar la autenticación.</dd>
<dt>Llamada de teléfono con pin</dt>
<dd>Con esta opción seleccionada, escriba un valor de pin en el portal de cliente. El pin debe tener entre 4 y 8 números. Cuando intente iniciar sesión en el portal, recibirá una llamada en el número principal listado en el portal. Cuando conteste, se le indicará que escriba su número de pin seguido de # para completar la autenticación.</dd>
<dt>SMS y pin puntual</dt>
<dd>Con esta opción seleccionada, recibirá un mensaje de texto con un pin que utilizará para responder al mensaje. Cuando escriba el pin proporcionado, se completará el proceso de autenticación y le registrará en el portal.</dd>
<dt>Texto SMS con valor puntual y pin</dt>
<dd>Con esta opción seleccionada, se crea un valor de pin de 4 a 8 números. Recibirá un mensaje de texto, y usted responderá con el código proporcionado y el número de pin sin espacios.</dd>
<dt>App de PhoneFactor y estándar (sin pin)</dt>
<dd>Abra la aplicación PhoneFactor (Azure Authenticator) en el dispositivo y pulse <strong>Autenticar</strong>. Mostrará que se ha autenticado correctamente utilizando PhoneFactor y le registrará en el portal.</dd>
<dt>App de PhoneFactor con pin</dt>
<dd>Con esta opción, establezca un pin, de entre 4 y 8 números, en el portal. A continuación, abra la aplicación PhoneFactor (Azure Authenticator) en el dispositivo. A continuación, especifique el pin que se ha creado en el portal y pulse <strong>Autenticar</strong> para iniciar sesión en el portal.</dd>
</dl>

## Cambio del estado de un usuario
{: #cp_changeuserstat}

Su estado en el portal de cliente determinará su accesibilidad al portal del cliente. Entre las categorías de estado que puede actualizar en la cuenta se encuentran Activo, Inhabilitado y Solo VPN. El estado puede ser modificado por diversas razones y el estado se puede actualizar en cualquier momento. Entre las categorías de estado del cliente se incluyen aquellas que los usuarios pueden actualizar y aquellas actualizadas automáticamente. Incluyen lo siguiente:
<dl>
<dt>Activo</dt>
<dd>El usuario tiene acceso completo al portal del cliente y a VPN basado en permisos establecidos por el administrador de la cuenta. Este estado se puede seleccionar o modificar manualmente en cualquier momento.</dd>
<dt>Inhabilitado</dt>
<dd>El usuario no tiene acceso a ningún permiso ni suscripción en la cuenta, incluido el portal del cliente y VPN. Si otro usuario de la cuenta establece la categoría de estado en inhabilitado, este estado puede ser seleccionado manualmente o cambiado en cualquier momento.</dd>
<dt>Solo VPN</dt>
<dd>El usuario tiene acceso completo a la conectividad de VPN, en función de su conjunto de permisos, pero no puede acceder al portal de clientes. Este estado se puede seleccionar o modificar manualmente en cualquier momento.</dd>
<dt>Inactivo</dt>
<dd>El usuario no ha accedido al portal de clientes ni a VPN en los últimos 60 días. Este es un estado generado por el sistema.</dd>
<dt>cancel_pending</dt>
<dd>Un administrador de la cuenta ha cancelado a este usuario y la cancelación se está procesando en este momento. Este es un estado generado por el sistema.</dd>
</dl>

Efectúe los pasos siguientes para cambiar el estado de un usuario en el portal del cliente.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Usuarios** en la barra de navegación.
3. Seleccione **Cambiar estado de usuario** en la lista **Acciones**.
4. En la lista **Estado**, seleccione el estado adecuado según las definiciones de la lista anterior.
5. Pulse **Guardar**.

Después de actualizar el estado de un usuario, los cambios en la accesibilidad del portal de clientes se alinean con el nuevo estado.

## Edición del acceso VPN de un usuario
{: #cp_edituservpnaccess}

Cuando [se añade un usuario nuevo](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct) a una cuenta de portal de clientes, se selecciona el acceso VPN desde diversos métodos de conexión, incluidos SSL, PPTP, o una combinación de ambos. Con el acceso VPN, se puede acceder a la red privada en su totalidad o el acceso a la red se puede limitar a una o varias subredes específicas. Puede gestionar y actualizar el acceso a VPN en cualquier momento desde la ventana Usuarios. Efectúe los pasos siguientes para editar el acceso VPN de un usuario.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Acceso VPN** en la barra de navegación.
3. En la columna **Acceso VPN** para el usuario, pulse el enlace del tipo de acceso VPN actual para visualizar la ventana Acceso VPN.
4. En la lista **Tipo de VPN**, seleccione un método VPN (SSL, PPTP, SSL y PPTP, o ninguno) para asignar el usuario.
5. Indique cómo debería gestionarse el **Acceso de subred**:
  * Seleccione **Automático** para gestionar automáticamente el acceso de subred
  * Seleccione **Manual** para gestionar manualmente el acceso de subred y, a continuación, marque el recuadro de selección **Otorgar acceso** para cada subred a la que debería tener acceso el usuario. Asegúrese de desmarcar los recuadros de selección a los que el usuario no debería tener acceso.
6. Pulse **Guardar**.

Después de actualizar el acceso VPN de un usuario, sus permisos se actualizarán en consecuencia y la columna Acceso VPN mostrará el método de acceso VPN actualizado, si procede.

### Activación o desactivación del acceso VPN
{: #cp_pptpvpn}

Puede activar PPTP VPN para formar un túnel seguro en la red privada de la infraestructura de {{site.data.keyword.BluSoftlayer_full}} utilizando el software especializado de cliente que se ejecuta en el escritorio o en el dispositivo dedicado. Puede utilizar PPTP si necesita conectar toda su oficina o si no puede utilizar la solución SSL VPN.

Se le asignará una conexión PPTP con conexiones adicionales disponibles.  Puede solicitar soporte para permitir acceso ilimitado a PPTP, que está disponible sin coste adicional. Utilice los pasos siguientes para activar o desactivar el acceso PPTP VPN:

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Acceso VPN** desde la barra de menús.
3. En la columna **Acceso VPN** para el usuario, pulse el enlace del tipo de acceso VPN actual para visualizar la ventana Acceso VPN.
4. En la lista **Tipo de VPN**, seleccione un método VPN (SSL, PPTP, SSL y PPTP, o ninguno) para asignar el usuario.

## Establecimiento de la opción Soporte en la UE
{: #cp_seteusupported}

Puede indicar que desea soporte exclusivamente de un equipo de soporte ubicado físicamente en la Unión Europea (UE). Puede seleccionar esta opción al configurar su cuenta o al actualizar la cuenta existente. Para establecer la opción **Soporte en la UE**, siga estos pasos:
1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Pulse **Cuenta** > **Gestionar** > **Perfil de la empresa** desde la barra de menús.
3. Marque el recuadro de selección **Soporte en la UE**.
4. Pulse **Solicitar actualización del perfil**.

Si la opción **Soporte en la UE** no está disponible, podría tener usuarios en su cuenta con el acceso PPTP VPN habilitado. Inhabilite el acceso PPTP VPN para todos los usuarios de su cuenta en primer lugar para poder habilitar la opción **Soporte en la UE**. Consulte [Activación o desactivación del acceso PPTP VPN](/docs/customer-portal/cpmanuserprof.html#cp_pptpvpn) para obtener más información.

Para obtener más información sobre la implementación de la opción **Soporte en la UE** al abrir una incidencia de soporte, consulte [Solicitud de soporte para recursos en la Unión Europea](/docs/get-support/howtogetsupport.html#eusupported).
