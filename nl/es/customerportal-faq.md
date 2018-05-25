---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Preguntas más frecuentes
{: #bicpfaq}

Las siguientes preguntas frecuentes se relacionan con la gestión de problemas de recursos de infraestructura.
{:shortdesc}


## ¿Cómo puedo recuperar mis credenciales para el Portal de clientes?
{: #bicp_retcreds}

Si utiliza IBMid para la autenticación, cuando realice su primer pedido o cuando se le añada como usuario a una cuenta, se enviará un correo electrónico que tiene un enlace para iniciarle a su IBMid. Si pierde u olvida el nombre de usuario o la contraseña, vaya al [perfil de IBMid ![Icono de enlace externo](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} y restablezca o recupere la contraseña utilizando las instrucciones que siguen al signo en curso. Se le solicitará que especifique la información específica, lo que podría incluir proporcionar respuestas a las preguntas de seguridad.

Si NO utiliza IBMid para la autenticación, cuando realice su primer pedido o cuando se le añada como usuario a una cuenta de [portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, recibirá un correo electrónico que contiene su nombre de usuario y su contraseña inicial para empezar en el portal del cliente. Asegúrese de cambiar la contraseña después de iniciar sesión por primera vez editando su perfil de usuario. Para cambiar la contraseña, inicie sesión con la información del correo electrónico y pulse su nombre de usuario en el panel superior para editar su perfil.

Si olvida la contraseña tras iniciar sesión, utilice la característica **Contraseña olvidada** que está disponible en la pantalla de inicio de sesión del [portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Se le solicitará que especifique información específica, incluido un conjunto de pregunta que ha especificado al editar el perfil de usuario.

Si olvida su nombre de usuario, póngase en contacto con el administrador de la cuenta o con el usuario maestro, que tienen la capacidad de recuperar su nombre de usuario. Si usted es el administrador o el usuario maestro de la cuenta, póngase en contacto con el Soporte para obtener ayuda adicional.

## ¿Qué es el IBMid, y cómo se relaciona con los usuarios de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_whatisibmid}

Las cuentas nuevas requieren IBMid para la autenticación. Las cuentas existentes seguirán utilizando el nombre de usuario y la contraseña de SoftLayer para la autenticación hasta que ejecute la herramienta de migración para cambiar a un IBMid. Su cuenta de SoftLayer tiene un usuario maestro, que tendrá autorización para añadir más usuarios dentro de esa misma cuenta. Consulte [Cómo se gestionan las cuentas de SoftLayer en el portal del cliente](/docs/customer-portal/cphowacctsman.html) para obtener más información.

## ¿Cómo puedo enlazar una cuenta de SoftLayer existente?
{: #bicp_linkbmxacct}

Si usted es el usuario maestro de la cuenta de SoftLayer, inicie sesión en el portal del cliente y pulse **Enlazar una cuenta** en la cabecera.  Consulte [Cómo enlazar cuentas de usuario de IBMid](/docs/account/softlayerlink.html) para obtener más información.

## ¿Tengo que ser un usuario existente de {{site.data.keyword.Bluemix_notm}} para enlazar cuentas?
{: #bicp_bmxusertolink}

No. Puede crear una cuenta nueva de {{site.data.keyword.Bluemix_notm}} o enlazar una cuenta de prueba o de pago según uso existente de {{site.data.keyword.Bluemix_notm}}.


## ¿Cómo funcionará mi autenticación de dos factores?
{: #bicp_2fa}

No hay impacto en la configuración de la autenticación de dos factores a nivel de cuenta. La autenticación de dos factores no es por IBMid; sigue siendo por cuenta. Cuando un IBMid se asocie con muchas cuentas, y pueda cambiar entre ellas, debe confirmar su identidad cada vez que cambie a una cuenta distinta que necesite la autenticación de dos factores. Esto es cierto incluso aunque la cuenta anterior y la cuenta nueva estén configuradas con el mismo mecanismo de 2FA.

Para obtener más información sobre IBMid con la autenticación de dos factores, consulte [Uso de la autenticación de dos factores en cuentas enlazadas](/docs/account/softlayerlink.html).


## ¿Quién puede enlazar cuentas?
{: #bicp_wholinkaccts}

Solo los usuarios maestros de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} pueden enlazar cuentas de SoftLayer y de {{site.data.keyword.Bluemix_notm}}. El correo electrónico de un usuario maestro también debe estar asociado al propietario principal de la cuenta de {{site.data.keyword.Bluemix_notm}} que se está enlazando.


## ¿Qué utilizaré para iniciar sesión en cada portal?
{: #bicp_logineachport}

La facturación de la cuenta está enlazada y puede moverse de forma sencilla entre las cuentas de SoftLayer y {{site.data.keyword.Bluemix_notm}}, pero sus identidades de cuenta permanecerán separadas.

* Si la cuenta no utiliza IBMid para la autenticación, siga utilizando el ID de SoftLayer para los productos y servicios de SoftLayer, y utilice IBMid para los productos y servicios de {{site.data.keyword.Bluemix_notm}}.

* Si la cuenta utiliza IBMid para la autenticación, utilice el IBMid para acceder a las cuentas de SoftLayer y {{site.data.keyword.Bluemix_notm}}.


## He intentado iniciar sesión con mi nombre de usuario de SoftLayer, ¿por qué obtengo un error?
{: #bicp_SLloginerror}

Tras cambiar a un IBMid, si inicia sesión en el portal del cliente con el nombre de usuario de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}, verá el error *"Se han proporcionado credenciales de inicio de sesión no válidas"*.
Esto se debe a que, tras cambiar a un IBMid, ya no puede iniciar sesión en el portal del cliente con su nombre de usuario de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Debe pulsar **Iniciar sesión con IBMid** en el diálogo Inicio de sesión de cuenta.

## He intentado iniciar sesión con mi IBMid, ¿por qué obtengo un error?
{: #bicp_IBMidloginerror}

Al iniciar sesión con su IBMid, si obtiene el error *"No hemos reconocido este IBMid o correo electrónico"*, asegúrese de que está especificando una dirección de correo electrónico completa. Asegúrese también de que no está utilizando el nombre de usuario de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.


##  Tengo una cuenta nueva de SoftLayer que utiliza IBMid para la autenticación; ¿puedo utilizar el mismo ID para la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} y {{site.data.keyword.Bluemix_notm}}?
{: #bicp_loginIBMidSLBlusame}

Sí, puede utilizar el mismo IBMid para iniciar sesión en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} y en {{site.data.keyword.Bluemix_notm}}.


## He enlazado una cuenta de {{site.data.keyword.Bluemix_notm}}, ¿cómo puedo dar acceso al resto de los miembros del equipo de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_linkgiveteamaccess}

Debe invitarles a {{site.data.keyword.Bluemix_notm}}. En la interfaz de usuario de {{site.data.keyword.Bluemix_notm}}, seleccione **Cuenta y soporte** > **Cuenta** > **Invitar a miembros del equipo**. Después de haber seleccionado un grupo de recursos, verá una opción para añadir los miembros del equipo de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Puede que tenga que iniciar sesión en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para poder enviar invitaciones. {{site.data.keyword.Bluemix_notm}} obtiene la lista de usuarios de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}, y a continuación puede seleccionar qué usuarios invitar a la cuenta de {{site.data.keyword.Bluemix_notm}}.


## ¿Dónde está mi correo electrónico para completar el cambio a IBMid?
{: #bicp_ibmidswitchemail}

Si ha seguido el asistente para cambiar a IBMid y no ha recibido el correo electrónico, el envío del correo electrónico con su código de registro puede tardar desde unos minutos a unas horas. Puede volver a la página **Editar perfil de usuario** en el portal del cliente y pulsar **Reenviar correo electrónico** para intentarlo de nuevo.


## ¿Tendré acceso completo y acceso como usuario root a mi cuenta?
{: #bicp_fullrootaccaccess}

Los usuarios maestros, y aquellos con permisos de administrador, tienen acceso completo como usuario root a las cuentas del portal y de la API del cliente. Los usuarios sin permisos de administrador tienen la accesibilidad controlada por aquellos con roles de administración. Estos permisos los pueden actualizar administradores desde el portal de cliente [editando un perfil de usuario](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Sin permisos de administrador, puede editar el perfil de usuario en el portal de cliente pulsando su nombre de usuario en el panel superior.


## ¿Puedo enlazar una cuenta de suscripción de {{site.data.keyword.Bluemix_notm}}?
{: #bicp_linkbmxsubacct}

Todas las cuentas vinculadas en {{site.data.keyword.Bluemix_notm}} deben ser cuentas de pago según uso. Puede crear una cuenta nueva de pago según uso o enlazar una cuenta de pago según uso existente. O bien, puede enlazar una cuenta de prueba existente, pero se actualizará a una cuenta de pago según uso.


## ¿Cómo puedo desenlazar mi cuenta de {{site.data.keyword.Bluemix_notm}} con mi cuenta de infraestructura de {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_unlinkacct}

Después de enlazar las cuentas, estas no se podrán desenlazar.


## ¿Qué es mi perfil de empresa y dónde puedo encontrarlo?
{: #bicp_whatfindcompprof}

El perfil de empresa era la información enviada en el momento de crear la cuenta e incluye un contacto principal para la empresa, junto con el nombre, la dirección y el número de teléfono de la empresa. Esta información se utiliza por diversos motivos y se debe mantener actualizada en todo momento. Para ver el perfil de la empresa para su cuenta o para solicitar cambios, consulte [Actualización del perfil de la empresa](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch).

## ¿Dónde puedo encontrar las contraseñas de mi dispositivo y del software?
{: #bicp_devswpw}

Las contraseñas del dispositivo y del software se almacenan en dos ubicaciones dentro del [portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Para recuperar las credenciales del dispositivo, incluidos el nombre de usuario y la contraseña del administrador y del usuario root para {{site.data.keyword.baremetal_short}} y {{site.data.keyword.virtualmachinesshort}}, consulte [Interactuar con un dispositivo en la vista de instantánea](/docs/vsi/vsi_interact_device_snapshot_view.html). Para ver y recuperar rápidamente las credenciales del software que se rastrean manualmente utilizando el portal del cliente, consulte [Gestión el acceso a dispositivos](/docs/vsi/vsi_device_access.html).

## ¿Cómo mantengo mis datos web sincronizados?
{: #bicp_webdatasync}

Aunque es responsable de mantener la coherencia de datos entre los servidores reales, {{site.data.keyword.BluSoftlayer_full}} proporciona una red privada que puede utilizar para sincronizar sin incurrir en cargos de uso.


## ¿Qué es el Event Management System?
{: #bicp_whatisems}

Event Management System es un conjunto de herramientas que optimiza la forma en que {{site.data.keyword.BluSoftlayer_full}} comparte la información con los usuarios sobre problemas de infraestructura no planificados y sucesos próximos de mantenimiento planificados. Utiliza alertas por correo electrónico basadas en suscripción y con destino para estos incidentes para compartir el tipo de suceso que se haya producido. Proporciona a los usuarios suscritos detalles adicionales sobre el impacto general del suceso y un estado actual del incidente en curso no planificado (UIP).

## ¿Cómo y dónde puedo cancelar un dispositivo?
{: #bicp_candev}

Puede cancelar un dispositivo en cualquier momento a través del [portal del cliente ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Consulte [Cancelar un dispositivo](/docs/vsi/vsi_managing.html) para obtener más información sobre la finalización de una solicitud de cancelación.
