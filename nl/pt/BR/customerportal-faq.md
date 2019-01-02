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
{:faq: data-hd-content-type='faq'}


# FAQ
{: #bicpfaq}

## Como recupero minhas credenciais para o portal do cliente?
{: #bicp_retcreds}
{: faq}

Se você usar o IBMid para autenticação, quando fizer seu primeiro pedido ou quando for incluído como um usuário em uma conta, você receberá um e-mail com um link para começar a usar seu IBMid. Se você perder ou esquecer seu nome de usuário ou senha, acesse seu [perfil do IBMid ![Ícone de link externo](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} e reconfigure ou recupere a senha. Você é solicitado a inserir informações específicas, o que pode incluir a criação de respostas para suas perguntas de segurança.

Se você não usar o IBMid para autenticação ao fazer seu primeiro pedido ou ser incluído como um usuário em uma conta do [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, você receberá um e-mail com seu nome de usuário e senha inicial para iniciar no portal do cliente. Certifique-se de mudar sua senha após efetuar login pela primeira vez editando seu perfil do usuário.

Se você esquecer sua senha depois de efetuar login, use o recurso **Senha esquecida ** que está disponível na tela de login do portal do cliente. Será solicitado que você insira informações específicas, incluindo um conjunto de perguntas de segurança especificadas ao configurar seu perfil de usuário.

Se você esquecer seu nome de usuário, entre em contato com o administrador da conta ou com o usuário principal, que poderão recuperá-lo. Se você for o administrador ou o usuário principal na conta, entre em contato com o Suporte para obter mais assistência.

## Qual é o IBMid?
{: #bicp_whatisibmid}
{: faq}

Novas contas requerem o IBMid para autenticação. As contas existentes continuam usando o nome de usuário e a senha do SoftLayer para autenticação até que você execute a ferramenta de migração para alternar para um IBMid. Sua conta do SoftLayer tem um usuário principal que tem autoridade para incluir mais usuários dentro dessa mesma conta. 

## Como vincular uma conta do SoftLayer existente?
{: #bicp_linkbmxacct}
{: faq}

Se você for o usuário principal na conta do SoftLayer, efetue login no portal do cliente e clique em **Vincular uma conta** no cabeçalho. Veja [Vinculando contas do usuário IBMid](/docs/account/softlayerlink.html) para obter informações adicionais.

## Devo ser um usuário existente do {{site.data.keyword.Bluemix_notm}} para vincular contas?
{: #bicp_bmxusertolink}
{: faq}

Não. É possível criar uma nova conta do {{site.data.keyword.Bluemix_notm}} ou vincular uma conta existente do {{site.data.keyword.Bluemix_notm}} Lite ou pré-paga.

## Como a autenticação de dois fatores funciona?
{: #bicp_2fa}
{: faq}

Não há nenhum impacto na configuração de autenticação de dois fatores (2FA) no nível da conta. A 2FA não é por IBMid; ainda é por conta. Quando um IBMid está associado a muitas contas e você alterna entre elas, deve-se confirmar sua identidade toda vez que alterna para uma conta diferente que requer 2FA. Isso é verdadeiro mesmo caso a conta anterior e a nova conta sejam ambas configuradas com o mesmo mecanismo de 2FA.

Para obter mais informações sobre o IBMid com 2FA, consulte [Uso de autenticação de diversos fatores em contas vinculadas](/docs/account/softlayerlink.html#2fa).

## Quem pode vincular contas?
{: #bicp_wholinkaccts}
{: faq}

Somente usuários principais da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} podem vincular contas do SoftLayer e do {{site.data.keyword.Bluemix_notm}}. O e-mail de um usuário principal também deve estar associado ao proprietário principal da conta do {{site.data.keyword.Bluemix_notm}} que está sendo vinculada.

## O que eu usarei para efetuar login em cada console?
{: #bicp_logineachport}
{: faq}

O faturamento de sua conta está vinculado e você pode mover facilmente entre as contas do SoftLayer e do {{site.data.keyword.Bluemix_notm}}, mas as suas identidades de conta permanecem separadas.

* Se a sua conta não usar o IBMid para autenticação, continue usando o ID do SoftLayer para produtos e serviços do SoftLayer e seu IBMid para produtos e serviços do {{site.data.keyword.Bluemix_notm}}.

* Se sua conta usa o IBMid para autenticação, use seu IBMid para acessar os ambas as contas do SoftLayer e do {{site.data.keyword.Bluemix_notm}}.

## Por que recebo um erro ao tentar efetuar login com meu nome de usuário do SoftLayer?
{: #bicp_SLloginerror}
{: faq}

Depois de alternar para um IBMid, se você efetuar login no portal do cliente com seu nome de usuário da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}, o erro "Credenciais de login inválidas fornecidas" será exibido. Depois de alternar para um IBMid, não é mais possível efetuar login no portal do cliente com seu nome do usuário da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Deve-se clicar em **Login com IBMid** no diálogo de Login da Conta.

## Por que recebo um erro ao tentar efetuar login com meu IBMid?
{: #bicp_IBMidloginerror}
{: faq}

Ao efetuar login com seu IBMid, o erro "Não reconhecemos esse IBMid ou e-mail" é exibido. Certifique-se de inserir um endereço de e-mail completo. Além disso, certifique-se de que não esteja usando o seu nome de usuário da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}.

## Os membros da equipe de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} podem acessar minha conta vinculada?
{: #bicp_linkgiveteamaccess}
{: faq}

Deve-se convidá-los para o {{site.data.keyword.Bluemix_notm}}. No console do {{site.data.keyword.Bluemix_notm}}, clique em **Gerenciar** > **Conta** > **Usuários**. Depois de selecionar um grupo de recursos, será possível incluir os membros da equipe de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Talvez seja necessário efetuar login no portal do cliente antes de poder enviar convites. O {{site.data.keyword.Bluemix_notm}} obtém a lista de usuários de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} e, em seguida, é possível selecionar quais usuários convidar para a conta do {{site.data.keyword.Bluemix_notm}}.

## Onde está meu e-mail para concluir a comutação para o IBMid?
{: #bicp_ibmidswitchemail}
{: faq}

Se você seguiu o assistente para alternar para o IBMid e não recebeu o e-mail, poderá levar de minutos a horas para que o e-mail com seu código de registro seja enviado a você. É possível voltar para a página **Editar perfil do usuário** no portal do cliente e clicar em **Reenviar e-mail** para tentar novamente.

## Eu terei acesso raiz total à minha conta?
{: #bicp_fullrootaccaccess}
{: faq}

Os usuários principais e aqueles com permissões de administrador têm acesso raiz completo às contas no portal do cliente e à API. Os usuários sem permissões de administrador têm acessibilidade que é controlada por aqueles com funções administrativas. Essas permissões podem ser atualizadas pelos administradores do portal do cliente [editando um perfil do usuário](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Sem permissões de administrador, é possível editar seu perfil do usuário no portal do cliente clicando em seu nome do usuário no painel superior.

## Posso vincular uma conta de Assinatura do  {{site.data.keyword.Bluemix_notm}} ?
{: #bicp_linkbmxsubacct}
{: faq}

Todas as contas vinculadas no {{site.data.keyword.Bluemix_notm}} devem ser contas Lite ou pré-pagas. 

## Como desvinculo minha conta?
{: #bicp_unlinkacct}
{: faq}

Depois que as contas são vinculadas, não é possível desvinculá-las.


## O que é o perfil da minha empresa e onde posso localizá-lo?
{: #bicp_whatfindcompprof}
{: faq}

O perfil da empresa são as informações enviadas no momento em que a conta é criada e inclui um contato principal para sua empresa, junto ao nome, endereço e número do telefone da empresa. Essas informações são usadas por várias razões e devem ser mantidas sempre atuais. Para visualizar o perfil da empresa para sua conta ou para solicitar mudanças, consulte [Atualizando o perfil de sua empresa](/docs/customer-portal/cpmanacctcompprofcont.html#cp_updcompprof).

## Onde localizar minhas senhas de dispositivo e software?
{: #bicp_devswpw}
{: faq}

As senhas do dispositivo e do software são armazenadas em dois locais dentro do portal do cliente. Para recuperar as credenciais do dispositivo, incluindo o nome do usuário raiz ou administrador e a senha para o {{site.data.keyword.baremetal_short}} e o {{site.data.keyword.virtualmachinesshort}}, consulte [Interagir com um dispositivo na visualização de captura instantânea](/docs/vsi/vsi_interact_device_snapshot_view.html). Para visualizar e recuperar rapidamente as credenciais de software rastreadas manualmente usando o portal do cliente, consulte [Gerenciando o acesso ao dispositivo](/docs/vsi/vsi_device_access.html).

## Como manter meus dados da web em sincronia?
{: #bicp_webdatasync}
{: faq}

Embora você seja responsável por manter a consistência de dados entre os servidores reais, o {{site.data.keyword.BluSoftlayer_full}} fornece uma rede privada que pode ser usada para sincronizar sem incorrer em encargos de uso.

## O que é o Sistema de Gerenciamento de Eventos?
{: #bicp_whatisems}
{: faq}

O Sistema de Gerenciamento de Eventos é um conjunto de ferramentas que otimiza a forma como o {{site.data.keyword.BluSoftlayer_full}} compartilha informações com usuários sobre problemas de infraestrutura não planejados e futuros eventos de manutenção planejados. Ele usa alertas de e-mail direcionados, baseados em assinatura, para esses incidentes para compartilhar o tipo de evento que ocorreu. Ele fornece usuários inscritos com detalhes sobre o impacto geral do evento e um status atual do incidente não planejado em andamento (UIP).

## Posso cancelar um dispositivo?
{: #bicp_candev}
{: faq}

É possível cancelar um dispositivo a qualquer momento por meio do portal do cliente. Consulte [Cancelar um dispositivo](/docs/vsi/vsi_managing.html) para obter mais informações sobre como concluir uma solicitação de cancelamento.
