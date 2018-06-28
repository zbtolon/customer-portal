---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Protección y escalado del entorno
{: #cp_compsegapptierssecscal}

Al alojar una aplicación, dos de los aspectos más críticos a tener en cuenta para cualquier administrador del sistema son la seguridad y la escalabilidad de la aplicación.
{:shortdesc}

## Protección de los sistemas con cortafuegos
{: #cp_bpsecuresystem}

Utilice los cortafuegos de hardware disponibles para asegurarse de que el dispositivo esté siempre protegido. Puede suministrar cortafuegos de hardware a petición sin tiempo de inactividad, si las reglas están establecidas correctamente, para proteger el servidor ante actividad no deseada.

Los cortafuegos son servicios complementarios para cualquier dispositivo que deba configurar y habilitar manualmente para asegurarse de que son efectivos. Puede bloquear los puertos superfluos e inhabilitar los puertos públicos para los sistemas basados en red privada para gestionar más la accesibilidad exterior a sus sistemas. Las exploraciones de vulnerabilidad regulares en el portal de cliente identifican cualquier riesgo de seguridad destacado o desconocido para poder mitigar los riesgos rápidamente.

Una vez que solicite el cortafuegos, debe habilitarlo y definir reglas.

### Activación del cortafuegos
{: #cp_bpnofirewalbypass}

La compra de un cortafuegos es un comienzo para proteger sus sistemas, pero solo comprarlo no le protege. Después de ser suministrado, el cortafuegos se encuentra en **modo de omisión** y no dispondrá de ninguna regla. Para que su cortafuegos se ejecute, debe crear reglas y activarlo para que pueda comenzar a bloquear la actividad no deseada.


## Protección del entorno segmentando los niveles de aplicación
{: #cp_copmsecenv}

Segmentar los niveles de aplicación lógica en capas de infraestructura física puede proporcionar mayor seguridad utilizando las listas de control de acceso (ACL). Al segmentar los niveles de aplicación, uno de los componentes más importantes a tener en cuenta es qué tráfico permite en cada capa de tráfico y desde dónde. Para determinar esta información, piense en cómo funciona básicamente la aplicación y qué servicios dependen entre sí para proporcionar a los usuarios su contenido solicitado.

Por ejemplo, piense en una aplicación de dos niveles que se basa en un frontal web y en un fondo de base de datos. Para esta aplicación, asegúrese de que el puerto 80 y 443 (si está utilizando SSL) están abiertos a Internet en los servidores web. Probablemente también desee bloquear todos los puertos a Internet y gestionar el servidor sobre VPN utilizando la red privada de infraestructura de {{site.data.keyword.BluSoftlayer_full}}. Probablemente también desearía desenlazar la dirección IP pública en el servidor de bases de datos y pasar todo el tráfico al mismo por el puerto 1433 (para MSSQL) o el puerto 3306 (para {{site.data.keyword.mysql}}) desde el servidor web. Gestionaría el servidor de base de datos en la red privada como el servidor web. También podría configurar un cortafuegos de software en el servidor de bases de datos para bloquear todo el tráfico desde el servidor web a los puertos de bases de datos específicos.

Al configurar el entorno de esta forma, impidiendo el acceso a SSH o RDP desde Internet e inhabilitando todo el tráfico de Internet a la base de datos, se aumenta la seguridad. La creación de ACL entre la capa web y la capa de base de datos hace más difícil el compromiso de la base de datos si el servidor web se ve comprometido.

## Escalado de su entorno segmentando los niveles de aplicación
{: #cp_copmscaleenv}

Un entorno de varias capas también proporciona facilidad de escalabilidad en comparación con las arquitecturas de host verticales o únicas. Puede configurar un entorno de varias capas para facilitar el escalado de la aplicación permitiendo el escalado para los servicios que necesitan más recursos. Por ejemplo, en el caso de ejemplo anterior, si el servidor web se ve desbordado, puede desplegar otro servidor web. A continuación, puede replicar los datos del sitio o de la aplicación y equilibrar la carga o configurar el DNS round robin para permitir que sus dos servidores web dividan la carga web. El DNS round robin o el equilibrio de carga proporciona una alta disponibilidad para su entorno permitiendo que varios servidores web respondan a las solicitudes entrantes. Si un único servidor cae, habrá otro nodo disponible para manejar las solicitudes de usuario.

También puede escalar la base de datos. Por ejemplo, con una base de datos {{site.data.keyword.mysql}}, una opción es configurar otro servidor físico y utilizarlo como un subordinado en una configuración de réplica {{site.data.keyword.mysql}}.  Puede segmentar todas las grabaciones de base de datos en el maestro y todas las lecturas en uno o varios subordinados para escalar la base de datos para dar soporte a más carga. Este tipo de configuración también añade un nivel de alta disponibilidad porque puede cambiar el estado de un subordinado a maestro. A continuación, puede direccionar el tráfico de lectura y de grabación en el subordinado si el nodo maestro de {{site.data.keyword.mysql}} cae.

Estas ideas son solo algunas de las muchas formas para proteger y escalar el entorno. Si tiene alguna pregunta o inquietud relacionadas con la mejor manera de diseñar su entorno desde una perspectiva de seguridad o de escalabilidad, la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} tiene un equipo de Ingeniería de ventas que puede ayudarle.
