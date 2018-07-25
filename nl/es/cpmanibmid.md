---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-10"

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:tip: .tip}
{:codeblock: .codeblock}
{:pre: .pre}
{:new_window: target="_blank"}

# Utilización de cuentas de IBMid con la infraestructura de {{site.data.keyword.BluSoftlayer_notm}}
{: #customerportal_ibmid}

La autenticación en la infraestructura de {{site.data.keyword.BluSoftlayer_notm}} ahora utiliza IBMid para proporcionar un inicio de sesión único para {{site.data.keyword.Bluemix_notm}}.
{:shortdesc}

Si tiene una cuenta existente de SoftLayer, puede cambiar a un IBMid. Un asistente de migración puede ayudar a guiarle a través de este conmutador. Para obtener más información, consulte [Cambio a un IBMid](/docs/account/softlayerlink.html#switching-to-ibmid).

## Correlación de varias cuentas de SoftLayer con un IBMid
{: #cp_mapmultclinfrto1ibmid}

Puede asociar un IBMid con varias cuentas de SoftLayer utilizando una dirección de correo electrónico de IBMid existente al configurar la cuenta. Solo se puede correlacionar un usuario de infraestructura de {{site.data.keyword.BluSoftlayer_notm}} para cada cuenta en el IBMid único. El IBMid debe ser exclusivo dentro de cada cuenta de SoftLayer. Sin embargo, un usuario con acceso a varias cuentas de SoftLayer puede utilizar un IBMid para acceder a varias cuentas de SoftLayer.

Por ejemplo, un IBMid puede correlacionar al usuario maestro en las cuentas A y B, y a otro usuario en las cuentas C y D. Una de las cuentas correlacionadas con dicho IBMid es la cuenta predeterminada. Normalmente, la cuenta predeterminada es la cuenta que se correlacionó por primera vez en el IBMid. Sin embargo, puede cambiar qué cuenta es la predeterminada utilizando una característica en el portal de clientes para cambiar cuentas.

![Varias cuentas de SoftLayer para un IBMid](images/ibmid-image.png)

Para un usuario con acceso de IBMid a varias cuentas con la autenticación de dos factores habilitada, se requerirá un código de verificación de autenticación de dos factores. El código de verificación es necesario, por cuenta, durante el inicio de sesión de la cuenta y cuando se cambia la cuenta predeterminada.
