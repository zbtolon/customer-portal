---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-12"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Adición de usuarios a una cuenta de SoftLayer
{: #customerportal_addusertocpacct}

Uno o varios usuarios pueden interactuar con los productos y servicios asociados con una cuenta. Si usted es el usuario maestro, puede añadir usuarios en cualquier momento.
{:shortdesc}

Si está gestionando los usuarios de la infraestructura de {{site.data.keyword.BluSoftlayer_full}}, qué cuentas de SoftLayer puede gestionar depende del acceso asignado a su cuenta de usuario y de cómo esté configurada la cuenta. Si usted es el usuario maestro, o si tiene acceso administrativo como propietario de una cuenta, puede gestionar el resto de los usuarios del portal del cliente. Si la cuenta no está configurada como un usuario maestro, puede gestionar el perfil de usuario.

En función de su acceso, puede gestionar su cuenta de SoftLayer o las cuentas de otros usuarios desde la ventana Usuarios. La ventana Usuarios del [portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} muestra los usuarios asociados con una cuenta. Las interacciones disponibles en la ventana Usuarios varían en función del permiso de cuenta exclusivo establecido.
  * Si usted es el usuario maestro de la cuenta, puede ver todos los usuarios asociados con la cuenta.

  Si debe compartir las credenciales de inicio de maestro para su cuenta, comparta las credenciales cuidadosamente. El inicio de sesión maestro permite controlar todos los aspectos de la cuenta y debería protegerse. Para permitir que otros usuarios utilicen el portal del cliente, puede configurar usuarios individuales o basados en permisos. De esa manera, podrá controlar quién puede interactuar con algunos aspectos de la cuenta.
  {:tip}
  * Si tiene acceso administrativo, puede ver todos los usuarios que ha creado y, si se le dio permiso a dichos usuarios para administrar otros usuarios, también puede ver los usuarios que han creado. También puede tomar acciones en cualquier usuario asociado con la cuenta, incluida la edición de acceso al portal de cliente, cambiar el estado de usuario y eliminar usuarios.
  * Si usted no es el usuario maestro de la cuenta y no tiene acceso administrativo, solo se mostrará el perfil. Puede interactuar con su propia cuenta, incluida la visualización de la clave de API, la edición del acceso VPN, y la adición de la autenticación externa.

Para gestionar usuarios desde la consola de {{site.data.keyword.Bluemix_notm}}, consulte la sección [Configuración de la cuenta](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) y [Gestión de identidad y acceso](/docs/iam/quickstart.html#getstarted). Consulte [Cómo funciona la consola de {{site.data.keyword.Bluemix_notm}}](/docs/overview/ui.html#ui) para obtener más información sobre la consola de {{site.data.keyword.Bluemix_notm}}.

Diferentes personas dentro de una organización tienen diferentes roles y responsabilidades, y los conjuntos de permisos de usuarios no son únicos. Por lo tanto, puede añadir usuarios al portal de cliente con roles para asegurarse de que cada persona o grupo tengan acceso únicamente a lo que deberían. Si los cambios se realizan en error o no estaban autorizados, puede rastrearlos de nuevo al usuario o al grupo para asegurarse de que pueda proporcionar permisos de usuario de formación o de actualización correctos. Esto minimiza el riesgo en diversas formas y permite a los usuarios centrarse en su rol especificado del portal de cliente.

Efectúe los pasos siguientes para añadir un usuario a una cuenta.

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse **Añadir usuario**.
4. Complete los campos necesarios en la sección **Información personal**, incluido el estado, un nombre de usuario y la dirección de correo electrónico para la comunicación y las notificaciones del portal de cliente, incluida la notificación inicial para configurar una contraseña para la cuenta.

  Opcionalmente, en lugar de especificar una dirección para el usuario, puede pulsar el recuadro de selección **Utilizar información predeterminada de la empresa** para rellenar la dirección de la empresa.
  {: tip}

5. Complete los campos necesarios en la sección **Valores de inicio de sesión**, incluido si los valores los puede editar el usuario, si la dirección IP está restringida, y si se necesita o no que el usuario configure y utilice preguntas de seguridad. Además, para los usuarios que no están utilizando IBMid, puede establecer la longitud de tiempo antes de que caduque la contraseña.
**Notas:**
* Si utiliza IBMid para la autenticación, actualice las contraseñas en los [perfiles de IBMid ![Icono de enlace externo](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} siguiendo las instrucciones debajo de **Iniciar sesión**.
* Pulse el recuadro de selección **Contraseña del portal de usuario para VPN** para sincronizar las contraseñas del portal de cliente y de VPN.
6. Pulse **Añadir usuario**.

Después de crear una cuenta para un usuario, el usuario recibirá una notificación por correo electrónico para terminar de configurar su cuenta estableciendo una contraseña y, opcionalmente, preguntas de seguridad, si indica que son necesarias.

La forma en que los usuarios sin acceso administrativo de un usuario maestro inician sesión en el portal del cliente dependerá del usuario maestro que haya proporcionado el acceso de usuario en sus cuentas de SoftLayer:
  * Si el usuario maestro tiene un IBMid para autenticarse, cada usuario que cree el usuario maestro tendrá un IBMid.
  * Si el usuario maestro tiene un ID de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para autenticar, cada usuario que cree el usuario maestro tendrá un nombre de usuario de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. El usuario maestro y cada usuario que cree el usuario maestro debe ejecutar la herramienta de migración para conmutar a un IBMid.
  * Si no se aplica ninguno de estos casos, en el caso de business partners de IBM por ejemplo, póngase en contacto con el Soporte para determinar qué ID de usuario utilizar.

## Establecimiento de los permisos de usuario en la cuenta
{: #cp_setuserpermsacct}

Efectúe los pasos siguientes para establecer los permisos para el usuario que acaba de añadir.

1. Pulse el icono **Permisos**, indicado por una figura de usuario con un candado.
2. Actualice los **Permisos de usuario** en todos los separadores para el nuevo usuario.
> **Nota:** Seleccione una opción desde la lista **Permisos rápidos** para ver conjuntos de permisos recomendados para tres tipos de usuarios. Pulse **Establecer permisos** para seleccionar el conjunto de permisos recomendado, o para personalizar la accesibilidad de los usuarios seleccionando opciones individuales en cada separador disponible.
3. Pulse **Añadir permisos de portal** para añadir los permisos o pulse **Restablecer permisos** para restablecer los permisos para el usuario.
4. Pulse el icono **Acceso de dispositivos**, indicado por tres servidores.
5. Pulse el recuadro de selección del dispositivo para cada dispositivo al que desee que acceda el usuario.
6. Pulse **Actualizar acceso de dispositivos** tras seleccionar los dispositivos.

Recibirá un correo electrónico con enlaces e información para guiarle a través de la creación de un IBMid para la autenticación en esta cuenta. Los pasos pueden incluir la creación de un nuevo IBMid si la cuenta está utilizando IBMid para la autenticación. La invitación caduca dentro de 7 días, pero puede ponerse en contacto con el administrador para reenviar la invitación.

Para todos los demás casos de autenticación, después de añadir el nuevo usuario, el usuario puede iniciar una sesión en el portal del cliente en cualquier momento para trabajar con diversos productos y servicios asociados con la cuenta. Puede desactivar el usuario en cualquier momento.
