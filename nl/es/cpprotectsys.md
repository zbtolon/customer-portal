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


# Protección de los sistemas
{: #customerportal_protsys}

Proteger los sistemas garantiza que los sistemas se ejecuten sin contratiempos y sin interrupciones innecesarias.

## Utilice la red privada
{: #cp_bpuseprivnet}

Puede gestionar sus dispositivos en el entorno lo más seguro posible utilizando la red privada de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Cuando sea posible, interactúe con sus dispositivos utilizando una conexión VPN y habilite la expansión de red para que los sistemas se comuniquen a través de la red privada. Para acceder a la red privada, edite el acceso VPN del usuario desde la [Lista de usuarios ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Utilice la lista [Red privada virtual ![Icono de enlace externo](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} para conectarse a una de las distintas opciones de VPN.

Para obtener más información sobre cómo utilizar una conexión VPN, consulte [Acerca de VPN](/docs/infrastructure/iaas-vpn/about-vpn.html).

### No deje RDP, SSH o los puertos de control en la red pública
{: #cp_bpnordpsshcponpubnet}

La red pública es idónea para muchas cosas pero ciertos aspectos, cuando se dejan disponibles en la red pública mediante puertos abiertos, pueden poner al sistema en situación de vulnerabilidad. Protéjase inhabilitando RDP o restringiendo SSH en la red pública. Si estos servicios deben estar disponibles en la red pública, piense en mover RDP o SSH a un número de puerto personalizado.

## Proteja los datos con copias de seguridad regulares
{: #cp_bpsafedataregback}

Planifique copias de seguridad para asegurarse de que los datos se almacenen de forma segura fuera del dispositivo y pueda cargarlos de nuevo si el dispositivo se pierde.

La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} ofrece varias soluciones de copia de seguridad para garantizar que pueda recuperar sus datos si la unidad falla o si el usuario realiza un error. Las soluciones de copia de seguridad actualmente incluyen NAS, copia de seguridad de EVault y CDP de R1Soft, que están disponibles en varias opciones de almacenamiento.
Por ejemplo, puede elegir uno de los siguientes servicios de copia de seguridad para almacenar los datos en una ubicación segura:
  * La copia de seguridad de EVault es un sistema de copia de seguridad automático basado en agente y una conocida solución automatizada de muy fácil activación (“set-and-forget”) para la gestión del dispositivo. Es compatible con el software de Microsoft que incluye Exchange y SQL mediante plug-ins. Los usuarios de EVault interactúan con este servicio a través de la aplicación basada en web WebCC de EVault.
  * R1Soft Continuous Data Protection (CDP) se puede instalar en el servidor o en una máquina virtual autogestionada. Puede utilizarlo si está buscando una única interfaz para gestionar todas sus copias de seguridad. Puede interactuar con R1Soft CDP a través de su propio sistema de gestión, lo que permite instalar agentes en máquinas virtuales y ofrece plugins de base de datos para obtener más funciones.

 Consulte la página [Almacenamiento ![Icono de enlace externo](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} para obtener más información sobre cada solución de copia de seguridad y consulte la [Guía de iniciación con servicios de copia de seguridad](/docs/infrastructure/Backup/index.html) para obtener más información sobre cómo realizar copias de seguridad de sus datos.

### No suponga que tenga redundancia; sabe que no
{: #cp_bpknowredundant}

La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} ofrece varias redundancias complementarias, que incluyen la vía de acceso dual, las fuentes de alimentación redundantes y las configuraciones RAID. Verifique que ha suministrado una o varias de estas características para garantizar que está trabajando en un entorno redundante y que está protegido si se produce un error.

### Confirme que la información está respaldada antes de recargar el sistema operativo
{: #cp_bpnoperfOSwobackupconf}

La recarga del sistema operativo elimina todos los datos del disco duro del dispositivo. Antes de iniciar una recarga de SO, realice una copia de seguridad de la información y verifique que se ha efectuado correctamente para no perder información. Una vez completada la recarga de SO, no podrá recuperarse la información perdida.

## No elimine Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} utiliza ASM para supervisar el estado de la matriz RAID. Si suprime este software, el equipo de soporte no podrá supervisar el dispositivo. Si ASM se elimina de su dispositivo, las alertas de anomalía de RAID en su dispositivo no estarán disponibles y no se le notificará de la anomalía a través del sistema de notificaciones automático.
