---

copyright:

  years: 2018

lastupdated: "2018-05-22"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Configuración de la autenticación de dos factores
{: #customerportal_2fa}

En el portal del cliente, se puede activar la autenticación externa de dos factores (2FA) para añadir protección extra al iniciar sesión en el portal. Esta capa extra de seguridad protege la cuenta de acceso no verificado, garantizando que los dispositivos, los datos y la información de cuenta estén protegidos.
{:shortdesc}

Si habilita la 2FA en el portal de cliente para su cuenta existente de SoftLayer, se le pedirá que especifique el código de seguridad cuando inicie sesión en la consola de {{site.data.keyword.Bluemix_notm}}. Sin embargo, la 2FA se aplica solo a los recursos de infraestructura en su cuenta de {{site.data.keyword.Bluemix_notm}}. Por lo tanto, puede realizar varias acciones en los recursos de su cuenta de {{site.data.keyword.Bluemix_notm}} sin llevar a cabo la 2FA.

2FA de la cuenta de SoftLayer no es por IBMid. Sigue siendo por cuenta. Cuando un IBMid está asociado con varias cuentas, y cambia entre ellas, debe confirmar su identidad cada vez que cambie a una cuenta distinta. Debe confirmar su identidad al cambiar entre cuentas, incluso si la cuenta anterior y la cuenta nueva están configuradas con el mismo mecanismo de 2FA.

## Habilitación de 2FA

La autenticación 2FA está disponible de dos formas. Es posible añadir ambos métodos de la autenticación externa por usuario por una pequeña tarifa mensual:

* Symantec Identify Protection es la herramienta de autenticación externa más comúnmente utilizada, que proporciona un código de seguridad dinámico que se utiliza además del nombre de usuario y de la contraseña al acceder al Portal del cliente.
* La autenticación de proporciona autenticación fuera de banda con una llamada telefónica, un SMS o una app para móvil.

 Si dispone de una cuenta enlazada, puede aprovechar la configuración de la autenticación de multifactores (MFA) [habilitando la autenticación de multifactores](/docs/iam/mfa.html) para su cuenta de {{site.data.keyword.Bluemix_notm}}.
 {: tip}

Para configura la autenticación 2FA, complete los pasos siguientes:

1. Acceda a la pantalla **Usuarios** en el portal de cliente.
2. Seleccione **Añadir autenticación externa** desde el menú **Acciones** para el usuario.
3. Complete los pasos siguientes en función del tipo de autenticación externa que se solicite:
    * Si elige Symantec Identity Protection, seleccione **Symantec Identity Protection** y especifique el ID de credencial de usuario.
    * Si elige PhoneFactor, seleccione **PhoneFactor**.
4. Pulse **Continuar**.
5. Siga las indicaciones en pantalla para el **Código promocional** y **Acuse de recibo de MSA**.
6. Pulse **Pedir autenticación externa** para completar el pedido. Pulse en **Cancelar** para cancelar la operación.

## Pasos siguientes
{: #2fanextsteps}

Después de añadir la autenticación externa para un usuario, los pasos siguientes dependen del tipo de autenticación.
* Si Symantec Identity Protection está habilitado, debe añadir el código de seguridad que está asociado con el ID de credenciales de usuario. Este código de seguridad es el código que se ha especificado en el sistema en el momento de añadir Symantec Identity Protection a la cuenta.
* Si PhoneFactor está habilitado, el usuario debe activar PhoneFactor para utilizar este tipo de autenticación de dos factores con la cuenta.

### Activación de la autenticación de PhoneFactor
{: #cp_actphonefacauth}

Después de añadir PhoneFactor, debe activar manualmente la autenticación externa con PhoneFactor a través del portal del cliente. Puesto que PhoneFactor utiliza contacto manual, es importante asegurarse de que todos los números de teléfono que están asociados con la cuenta estén siempre actualizados. No mantener actualizada la información de contacto puede provocar que no se pueda acceder al portal de cliente ni a VPN cuando PhoneFactor esté activo. Cuando PhoneFactor se haya añadido correctamente, recibirá un correo electrónico para confirmar que se ha añadido PhoneFactor. Tras recibir el correo electrónico, efectúe los pasos siguientes para activar la autenticación de PhoneFactor.

1. Acceda al portal de cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta > Usuarios** en la barra de navegación.
3. Pulse el nombre de usuario para acceder al perfil de usuario asociado para dicho usuario.
4. Desplácese a la sección **Valores de PhoneFactor**.

  Si la sección Valores de PhoneFactor no está disponible, compruebe en primer lugar que haya recibido el correo electrónico de suministro de PhoneFactor que indica que PhoneFactor se ha suministrado. Si se ha suministrado PhoneFactor y la sección no está disponible, cree una incidencia de soporte. Si PhoneFactor no se ha suministrado aún, espere el correo electrónico e inténtelo de nuevo.
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

Después de activar PhoneFactor, el portal de cliente o VPN necesita la autenticación a través de PhoneFactor. Después de autenticarse con las credenciales de usuario, un mensaje le indicará que se ha intentado dicha autenticación de PhoneFactor. Usted, o el usuario que está añadiendo, debe estar cerca del teléfono que está listado con PhoneFactor para completar la autenticación. PhoneFactor intentará autenticarse cinco veces. Tras cinco intentos de autenticación infructuosos, se le bloqueará durante aproximadamente una hora. Usted, o un usuario con acceso administrativo a la cuenta, puede cambiar los valores de autenticación de PhoneFactor en cualquier momento.  Usted, o un administrador de la cuenta, puede desactivar PhoneFactor en cualquier momento.

 Si elige configurar PhoneFactor para el portal de cliente y el inicio de sesión de la VPN, el resultado es dos procesos de inicio de sesión de 2FA independientes, uno para el portal de clientes y otro para VPN.
 {: tip}

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
<dd>Con esta opción seleccionada, cree un valor de pin de 4 a 8 números. Recibirá un mensaje de texto, y usted responderá con el código proporcionado y el número de pin sin espacios.</dd>
<dt>App de PhoneFactor y estándar (sin pin)</dt>
<dd>Abra la aplicación PhoneFactor (Microsoft Authenticator) en el dispositivo y pulse <strong>Autenticar</strong>. Muestra que se ha autenticado correctamente utilizando PhoneFactor y le registra en el portal.</dd>
<dt>App de PhoneFactor con pin</dt>
<dd>Con esta opción, establezca un pin, de entre 4 y 8 números, en el portal. A continuación, abra la aplicación PhoneFactor (Microsoft Authenticator) en el dispositivo. A continuación, especifique el pin que se ha creado en el portal y pulse <strong>Autenticar</strong> para iniciar sesión en el portal.</dd>
</dl>
