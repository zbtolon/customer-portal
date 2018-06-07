---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-24"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Configuración del inicio de sesión único
{: #customerportal_confssoserv}

Si usted es el usuario maestro de una cuenta o tiene acceso administrativo a la misma, puede configurar el inicio de sesión único. La configuración del inicio de sesión único para la infraestructura de {{site.data.keyword.BluSoftlayer_full}} es un proceso de dos pasos.  En primer lugar, seleccione y configure el proveedor de identidad. A continuación, configure la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para recibir la solicitud de autenticación del proveedor de identidad.
{:shortdesc}

## Selección y configuración del proveedor de identidad
{: #cp_setupidprov}

Si aún no tiene un proveedor de identidad, seleccione uno en primer lugar y configúrelo. Puede utilizar los siguientes proveedores de identidad con {{site.data.keyword.BluSoftlayer_notm}}:
* Ping Identity&reg;,
* OneLogin&trade;,
* IBM&reg; Cloud Security Enforcer,
* IBM Cloud Identity Services.
Póngase en contacto con el representante de ventas de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para obtener más información.

Si aún no tiene un proveedor de identidad configurado, puede ponerse en contacto con el soporte de proveedor de identidad para ver los pasos específicos. También puede utilizar los siguientes pasos de nivel superior para configurar el proveedor de identidad:
1. Prepare el entorno del proveedor de identidad descargando e instalando el archivo ejecutable.
2. Configure el proveedor de identidad para trabajar con la autenticación de {{site.data.keyword.BluSoftlayer_notm}}.

## Configuración de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para SSO
{: #cp_setupsso}

Debe extraer los siguientes campos necesarios de la información de metadatos de Security Assertion Markup Language&trade; (SAML&trade;) 2.0 del proveedor de identidad para utilizarlos con {{site.data.keyword.BluSoftlayer_notm}}.
<dl>
<dt>ID de entidad</dt>
<dd>El ID de entidad del proveedor de identidad.</dd>
<dt>URL de inicio de sesión único</dt>
<dd>El punto final del proveedor de identidad para SSO.</dd>
<dt>Certificado</dt>
<dd>El certificado de proveedor de identidad que se ha utilizado para firmar solicitudes.</dd>
</dl>

El campo siguiente es opcional:
<dl>
<dt>Huella dactilar de certificado</dt>
<dd>La huella dactilar del certificado. Este campo se puede utilizar en lugar del certificado completo.</dd>
</dl>

Efectúe los pasos siguientes para configurar la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para recibir la solicitud de autenticación del proveedor de identidad:
1. Inicie sesión en el proveedor de identidad, si aún no ha iniciado sesión, y localice la página **Configuración de SAML**. Tenga en cuenta la información siguiente:
  * ID de entidad
  * URL de inicio de sesión único
  * Certificado (los requisitos del certificado variarán en función de su proveedor de identidad).
2. Inicie sesión en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} como usuario maestro con el nombre y la contraseña del usuario maestro que ha utilizado para crear su cuenta de SoftLayer.
3. Pulse **Cuenta** > **Gestionar** > **Autenticación SAML**.
4. Escriba los metadatos del **Proveedor de identidad**.
5. Pulse **Guardar**.
6. Pulse **Cuenta** > **Gestionar** > **Autenticación SAML**.
7. Pulse **Descargar configuración XML** para descargar los metadatos del proveedor de servicio o anotar la información.
8. Utilice los metadatos del **Proveedor de servicio** para configurar su proveedor de identidad en función de las instrucciones del proveedor de identidad.  

Puede iniciar sesión en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} utilizando el ID federado. Para obtener más información acerca de los ID federados, consulte [Registro de {{site.data.keyword.Bluemix_notm}}](/docs/account/adminpublic.html) y la [Guía de adopción de federación empresarial de IBMid ![Icono de enlace externo](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}.
