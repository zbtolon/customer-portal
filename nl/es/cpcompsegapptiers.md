---

copyright:

  years: 1994, 2018

lastupdated: "2018-03-07"

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

Utilice los cortafuegos de hardware disponibles para asegurarse de que el dispositivo esté protegido en todo momento. Puede suministrar cortafuegos de hardware a petición sin tiempo de inactividad, si las reglas están establecidas correctamente, para proteger el servidor ante actividad no deseada.

Los cortafuegos son servicios complementarios para cualquier dispositivo que deba configurar y habilitar manualmente para asegurarse de que son efectivos. Puede bloquear los puertos superfluos e inhabilitar los puertos públicos para los sistemas basados en red privada para gestionar más la accesibilidad exterior a sus sistemas. La realización de exploraciones de vulnerabilidad regulares en el portal de cliente identifica cualquier riesgo de seguridad destacado o desconocido para poder mitigar los riesgos rápidamente.

Una vez que solicite el cortafuegos, debe habilitarlo y definir reglas.

### Activación del cortafuegos
{: #cp_bpnofirewalbypass}

La compra de un cortafuegos es un comienzo para proteger sus sistemas, pero solo comprarlo no le protege. Después de ser suministrado, el cortafuegos se encuentra en **modo de omisión** y no dispondrá de ninguna regla. Para que su cortafuegos se ejecute, debe crear reglas y activarlo para que pueda comenzar a bloquear la actividad no deseada.


## Protección del entorno segmentando los niveles de aplicación
{: #cp_copmsecenv}

Segmentar los niveles de aplicación lógica en capas de infraestructura física puede proporcionar mayor seguridad mediante el uso de listas de control de acceso (ACL). Al segmentar los niveles de aplicación, uno de los componentes más importantes a tener en cuenta es qué tráfico permite en cada capa de tráfico y desde dónde. Para determinar esto, deberá pensar en cómo funciona básicamente la aplicación y qué servicios dependen entre sí para proporcionar al usuario final su contenido solicitado.

Por ejemplo, con una aplicación de dos niveles que se basa en un frontal web y en un fondo de base de datos, deberá asegurarse de que el puerto 80 y 443 (si está utilizando SSL) están abiertos a Internet en los servidores web. Probablemente también desee bloquear todos los puertos a Internet y gestionar el servidor sobre VPN utilizando la red privada de infraestructura de {{site.data.keyword.BluSoftlayer_full}}. En este caso de ejemplo, probablemente desearía desenlazar la dirección IP pública en el servidor de bases de datos y pasar todo el tráfico al mismo por el puerto 1433 (para MSSQL) o el puerto 3306 (para {{site.data.keyword.mysql}}) desde el servidor web.  El servidor de bases de datos podría estar gestionado por la red privada al igual que el servidor web, y puede configurar un cortafuegos de software en el servidor de bases de datos para bloquear todo el tráfico desde el servidor web a los puertos de bases de datos específicos.

Al configurar el entorno de esta forma, se aumenta la seguridad impidiendo que las personas accedan a SSH o RDP desde Internet e inhabilitando todo el tráfico de Internet a la base de datos.  La creación de ACL entre la capa web y la capa de base de datos hace más difícil el compromiso de la base de datos en caso de que el servidor web se vea comprometido.

## Escalado de su entorno segmentando los niveles de aplicación
{: #cp_copmscaleenv}

Un entorno de varias capas también proporciona facilidad de escalabilidad en comparación con las arquitecturas de host verticales o únicas. Puede configurar un entorno de varias capas para facilitar el escalado de la aplicación permitiendo el escalado para los servicios que necesitan recursos adicionales. Por ejemplo, en el caso de ejemplo anterior, si el servidor web se ve desbordado, simplemente puede desplegar otro servidor web, replicar los datos del sitio o de la aplicación, y configurar el equilibrio de carga o el DNS round robin para permitir que sus dos servidores web dividan la carga web. El DNS round robin o el equilibrio de carga proporciona una alta disponibilidad para su entorno permitiendo que varios servidores web respondan a las solicitudes entrantes.  Si un único servidor cae, habrá otro nodo disponible para manejar las solicitudes de usuario final.

También puede escalar la base de datos. Por ejemplo, con una base de datos {{site.data.keyword.mysql}}, una opción es configurar otro servidor físico y utilizarlo como un ‘esclavo’ en una configuración de réplica maestro/esclavo de {{site.data.keyword.mysql}}.  Puede segmentar todas las grabaciones de base de datos en el ‘maestro’ y todas las lecturas en uno o varios ‘esclavos’ para escalar la base de datos para dar soporte a más carga.  Este tipo de configuración también añadirá un nivel de alta disponibilidad habilitando el cambio del estado de un ‘esclavo’ a ‘maestro’ y direccionará el tráfico de lectura y de escritura al mismo en el caso de que el nodo ‘maestro’ de {{site.data.keyword.mysql}} se caiga.

Estas ideas son solo algunas de las muchas formas para proteger y escalar el entorno. Si tiene alguna pregunta o inquietud relacionadas con la mejor manera de crear su entorno desde una perspectiva de seguridad o de escalabilidad, la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} tiene un equipo de Ingeniería de ventas que puede ayudarle.
