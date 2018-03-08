---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# API de SoftLayer
{: #customerportal_api}

Puede utilizar la API para interactuar con su cuenta, productos y servicios mediante llamadas de API directas en un entorno de desarrollo en lugar de utilizar el portal del cliente.
{:shortdesc}

El objetivo de la API es proporcionar un entorno donde puede completar cualquier tarea del portal del cliente en la API. El entorno de API se mantiene con adiciones y actualizaciones frecuentes para asegurarse de que tiene las mejores opciones disponibles, incluyendo la capacidad de programar en una variedad de idiomas y opciones para utilizar SOAP, XML-RPC y API basadas en REST. De forma similar a trabajar en el portal del cliente, si se hacen principalmente interacciones de cuenta en la API, necesita una fuente viable para el soporte también.

## ¿Cómo accedo a la API?
{: #cp_getapikey}

Puede acceder a la API con una clave de API específica de usuario. Las claves de API son identificadores alfanuméricos exclusivos que permiten acceder de forma segura a la API. La clave de API está enlazada específicamente el ID de usuario y proporciona los mismos permisos en la API que los que se tienen en el Portal de clientes. La clave de API solo se genera una vez y se puede recuperar y seguir utilizando. Efectúe los pasos siguientes para generar la clave de API:

1. Acceda al portal del cliente utilizando sus credenciales exclusivas.
2. Seleccione **Cuenta** > **Usuarios** en la barra de navegación.
3. Bajo la columna **CLAVE DE API** de la fila con las credenciales de usuario, pulse el enlace **Generar**.

Una vez generada la clave de API, el enlace **Generar** cambia a un enlace **Ver**, que puede utilizar para acceder a la clave de API en cualquier momento.

## ¿Dónde puedo obtener más información sobre la API?
{: #cp_apimoreinfo}

[SoftLayer Development Network (SLDN) ![Icono de enlace externo](../icons/launch-glyph.svg)](http://sldn.softlayer.com/){:new_window} está dedicado a darle soporte al interactuar con su cuenta, productos y servicios mediante la API. [SLDN ![Icono de enlace externo](../icons/launch-glyph.svg)](http://sldn.softlayer.com/){:new_window} contiene documentación sobre las API de SoftLayer, los lenguajes de programación soportados, las llamadas de API disponibles, etc. SLDN es el recurso a utilizar para obtener información sobre varias características de API, una lista completa de llamadas de API, y varias publicaciones de blog para darle ideas sobre cómo utilizar mejor la API.


Si tiene alguna pregunta sobre la API, puede publicarla en los foros de cliente o mediante comentarios directos de artículos.
