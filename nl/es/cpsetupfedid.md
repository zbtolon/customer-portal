---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-28"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Configuración de la federación de identidad
{: #cp_setupidfed}

Puede configurar la federación de identidad para habilitar un proveedor de servicios, como {{site.data.keyword.BluSoftlayer_full}} Infrastructure Management System (IMS), para consumir señales de seguridad generadas desde un sistema de identidad de confianza para fines de autenticación y autorización.
{:shortdesc}

Puede configurar la federación de identidad en SSO de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} de una de las formas siguientes:
* Creando usuarios en el proveedor de identidad y en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}
* Creando usuarios en el proveedor de identidad

Un rol define, para el proveedor de servicios, lo que el usuario está autorizado a hacer (mediante permisos) en su sistema después de que el usuario se haya autenticado. Por ejemplo, el rol *Usuario* podría tener permiso para ver solo distintas pantallas, pero no para actualizar ni añadir.

Pueden asignarse varios usuarios a un solo rol. Además, si existe un rol en el proveedor de identidad pero no en la infraestructura de {{site.data.keyword.BluSoftlayer}}, el usuario puede seguir iniciando sesión en la infraestructura de {{site.data.keyword.BluSoftlayer}} pero el usuario no tendrá ningún permiso asignado a un rol.
{: tip}


## Creación de usuarios en el proveedor de identidad y en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}
{: #cp_scenario1both}

En este modelo, ocurrirá lo siguiente:
* Los usuarios se crean tanto en el proveedor de identidad como en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}.
* Los permisos de usuario se asignan en IMS de la infraestructura de {{site.data.keyword.BluSoftlayer}} utilizando las API o el portal de clientes de la infraestructura de {{site.data.keyword.BluSoftlayer}}.
* Los usuarios se autentican con el proveedor de identidad y federan sus credenciales.
* La infraestructura de {{site.data.keyword.BluSoftlayer}} consume las credenciales y el control de acceso se basa en los permisos definidos para el usuario en IMS de infraestructura de {{site.data.keyword.BluSoftlayer}}.

Las cuentas para los usuarios que necesitan acceso a la infraestructura de {{site.data.keyword.BluSoftlayer}} se crean en primer lugar en la infraestructura de {{site.data.keyword.BluSoftlayer}} con contraseñas aleatorias. Todos los permisos deben configurarse en la infraestructura de {{site.data.keyword.BluSoftlayer}} antes de que el usuario pueda utilizar SSO a través del proveedor de identidad. Actualmente, los permisos se configuran basándose en el usuario individual.

### Configuración de un usuario
Efectúe los pasos siguientes para configurar un usuario:

1. [Adición de usuarios a una cuenta de SoftLayer](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. Asigne permisos en la infraestructura de {{site.data.keyword.BluSoftlayer}}.
3. Cree usuarios en el proveedor de identidad.

El campo **Correo electrónico** o **Nombre de usuario** dentro del perfil de usuario individual se utiliza para la señal Security Assertion Markup Language&trade; (SAML&trade;) 2.0. La señal correlaciona usuarios entre el proveedor de identidad y la infraestructura de {{site.data.keyword.BluSoftlayer}}.

### Flujo de ejemplo para la autenticación de inicio de sesión
{: #exlogauthflowidprovicloud}

El siguiente flujo de ejemplo muestra cómo podría funcionar la autenticación de inicio de sesión de usuario al crear usuarios en el proveedor de identidad y en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}:
1. El usuario accede al URL del proveedor de identidad desde una sesión de navegador.
2. El proveedor de identidad autentica el usuario, por ejemplo a través de su LDAP.
3. El proveedor de identidad devuelve respuestas de SAML 2.0.
4. El proveedor de identidad envía una respuesta SAML 2.0 al proveedor de servicios, en este caso la infraestructura de {{site.data.keyword.BluSoftlayer}}, para autenticar el ID de usuario.
5. La infraestructura de {{site.data.keyword.BluSoftlayer}} valida la respuesta de SAML 2.0.
6. El usuario inicia sesión en el portal de clientes de infraestructura de {{site.data.keyword.BluSoftlayer}} en función de la configuración de confianza entre el proveedor de identidad y la infraestructura de {{site.data.keyword.BluSoftlayer}}.


## Creación de usuarios en el proveedor de identidad
{: #cp_scenario2idp}

En este modelo, ocurrirá lo siguiente:
* Los roles se crean en el proveedor de identidad y se asignan al usuario.
* Las asignaciones de roles y permisos se configuran en IMS de la infraestructura de {{site.data.keyword.BluSoftlayer}} utilizando las API de infraestructura de {{site.data.keyword.BluSoftlayer}}.
* Los usuarios se autentican con el proveedor de identidad y federan sus credenciales y sus atributos de rol.
* La infraestructura de {{site.data.keyword.BluSoftlayer}} verifica las credenciales de usuario y los atributos de rol. Si los roles asignados a los usuarios por su proveedor de identidad coinciden con los roles de la infraestructura de {{site.data.keyword.BluSoftlayer}}, se otorgarán permisos a los usuarios para dichos roles cuando inicien sesión en la infraestructura de {{site.data.keyword.BluSoftlayer}}.
* Cuando el proveedor de identidad crea usuarios, estos se consideran como federados porque ellos, y sus roles, están autenticados a través de SAML 2.0.

### Configuración de un rol para un usuario
{: #cp_set-up-user-role}

Efectúe los pasos siguientes para configurar un rol para un usuario:

1. Configure los roles mediante la API de infraestructura de {{site.data.keyword.BluSoftlayer}}.
2. Configure los roles en el proveedor de identidad.
3. Asegúrese de que los roles definidos en la infraestructura de {{site.data.keyword.BluSoftlayer}} y en el proveedor de identidad tengan el mismo nombre.

### Configuración de un usuario
{: #setupuser}

Efectúe los pasos siguientes para configurar un usuario:

1. Configure los usuarios en el proveedor de identidad.
2. Asigne los roles a los usuarios del proveedor de identidad.

En este caso de ejemplo, no es necesario crear usuarios manualmente en la infraestructura de {{site.data.keyword.BluSoftlayer}}.

### Flujo de ejemplo para la autenticación de inicio de sesión de usuario
{: #exlogauthflowidprov}

El siguiente flujo de ejemplo muestra cómo podría funcionar la autenticación de inicio de sesión de usuario al crear usuarios en el proveedor de identidad:
1. El usuario accede al URL del proveedor de identidad desde una sesión de navegador.
2. El proveedor de identidad autentica el usuario, por ejemplo a través de su LDAP.
3. El proveedor de identidad devuelve respuestas de SAML 2.0.
4. El proveedor de identidad envía una respuesta SAML 2.0 al proveedor de servicios, en este caso la infraestructura de {{site.data.keyword.BluSoftlayer}}, para autenticar el rol de usuario.
5. La infraestructura de {{site.data.keyword.BluSoftlayer}} valida la respuesta de SAML 2.0.
6. La infraestructura de {{site.data.keyword.BluSoftlayer}} redirige al usuario al portal de clientes.
7. El usuario se registra en el portal de clientes de infraestructura de {{site.data.keyword.BluSoftlayer}}.

Revise los procedimientos del proveedor de identidad para establecer nuevos roles y asociarlos con la infraestructura de {{site.data.keyword.BluSoftlayer}}.
