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

# Usando as contas do IBMid com a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}
{: #customerportal_ibmid}

A autenticação na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} agora usa o IBMid para fornecer um único login para o {{site.data.keyword.Bluemix_notm}}.
{:shortdesc}

Se você tiver uma conta existente do SoftLayer, será possível alternar para um IBMid. Um assistente de migração pode ajudar a guiar você nessa alternância. Para obter mais informações, veja [Alternando para o IBMid](/docs/account/softlayerlink.html#switching-to-ibmid).

## Mapeando várias contas do SoftLayer para um IBMid
{: #cp_mapmultclinfrto1ibmid}

Será possível associar um IBMid a múltiplas contas do SoftLayer usando um endereço de e-mail do IBMid existente quando você configurar a conta. Apenas um usuário de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para cada conta pode ser mapeado para o IBMid único. O IBMid deve ser exclusivo dentro de cada conta do SoftLayer. No entanto, um usuário com acesso a várias contas do SoftLayer pode usar um IBMid para acessar as contas.

Um IBMid pode ser mapeado para o usuário principal nas contas A e B, por exemplo, e para outro usuário nas contas C e D. Uma das contas que é mapeada para esse IBMid é a conta padrão. Normalmente, a conta padrão é a conta que foi mapeada primeiro para o IBMid. No entanto, é possível alternar qual conta é a conta padrão usando um recurso no portal do cliente para alternar contas.

![Mapeando contas do SoftLayer para um IBMid](images/ibmid-image.png)

Para um usuário com acesso IBMid a várias contas com a autenticação de dois fatores (2FA) ativada, é necessário um código de verificação 2FA. De acordo com a conta, o código de verificação será necessário durante o login da conta e ao alternar a conta padrão.
