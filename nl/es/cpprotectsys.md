---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-04"

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

Puede gestionar sus dispositivos en el entorno lo más seguro posible utilizando la red privada de la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}. Cuando sea posible, interactúe con sus dispositivos utilizando una conexión VPN y habilite la expansión de red para que los sistemas se comuniquen a través de la red privada. Para acceder a la red privada, edite el acceso VPN del usuario desde la [Lista de usuarios ![Icono de enlace externo](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window}. Utilice las instrucciones de la [Red privada virtual ![Icono de enlace externo](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} para conectarse a una de las distintas opciones de VPN.

### No deje RDP, SSH o los puertos de control en la red pública
{: #cp_bpnordpsshcponpubnet}

La red pública es idónea para muchas cosas, pero hay ciertos aspectos que, cuando se dejan disponibles en la red pública mediante puertos abiertos, pueden poner al sistema en situación de vulnerabilidad. Protéjase inhabilitando RDP o restringiendo SSH en la red pública. Si estos servicios deben estar disponibles en la red pública, piense en mover RDP o SSH a un número de puerto personalizado.

## Proteja los datos con copias de seguridad regulares
{: #cp_bpsafedataregback}

La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} ofrece varias soluciones de copia de seguridad para garantizar que pueda recuperar sus datos en el caso de anomalía de la unidad o de error de usuario. Las soluciones de copia de seguridad actualmente incluyen NAS, copia de seguridad de EVault y CDP de R1Soft, que están disponibles con diversidad de opciones de almacenamiento. Consulte la página [Almacenamiento ![Icono de enlace externo](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} para obtener más información sobre cada solución de copia de seguridad.

### No suponga que haya redundancia; sabe que no
{: #cp_bpknowredundant}

La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} ofrece varias redundancias complementarias, incluidas la vía de acceso dual, las fuentes de alimentación redundantes y las configuraciones RAID. Verifique que ha suministrado una o varias de estas características para garantizar que está trabajando en un entorno redundante y que está protegido en caso producirse un error. 

### Confirme que la información está respaldada antes de realizar una recarga de SO
{: #cp_bpnoperfOSwobackupconf}

Recargar el sistema operativo elimina todos los datos del disco duro del dispositivo. Antes de iniciar una recarga de SO, realice una copia de seguridad de la información y verifique que se ha efectuado correctamente para no perder información. Una vez completada la recarga de SO, no podrá recuperarse la información perdida. 

## No elimine Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 La infraestructura de {{site.data.keyword.BluSoftlayer_notm}} utiliza ASM para supervisar el estado de la matriz RAID. Si suprime este software, el equipo de soporte no podrá supervisar el dispositivo. Si ASM se elimina de su dispositivo, las alertas de anomalía de RAID en su dispositivo no estarán disponibles y no se le notificará de la anomalía a través del sistema de notificaciones automático.
