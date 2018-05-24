---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-09"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# FAQ
{: #bicpfaq}

As perguntas mais frequentes a seguir se relacionam ao gerenciamento de problemas de recursos de infraestrutura.
{:shortdesc}


## Como recuperar minhas credenciais para o Portal do cliente?
{: #bicp_retcreds}

Se você usar o IBMid para autenticação, quando efetuar seu primeiro pedido ou quando for incluído como um usuário em uma conta, será enviado um e-mail com um link para você começar a usar seu IBMid. Se seu nome de usuário ou senha for perdida ou esquecida, acesse seu [perfil do IBMid ![Ícone de link externo](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} e reconfigure ou recupere a senha usando as instruções que seguem o processo de conexão. Será solicitado que insira informações específicas, que podem incluir o fornecimento de respostas às suas perguntas de segurança.

Se você NÃO usar o IBMid para autenticação, quando efetuar seu primeiro pedido ou for incluído como um usuário a uma conta do [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}, receberá um e-mail contendo seu nome de usuário e senha inicial para começar a usar o portal do cliente. Certifique-se de mudar sua senha após efetuar login pela primeira vez editando seu perfil do usuário. Para mudar sua senha, efetue login com as informações no e-mail e clique em seu nome do usuário no painel superior para editar seu perfil.

Se você esquecer sua senha após efetuar login, use o recurso **Esqueceu sua Senha** que está disponível na tela de login do [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Você será solicitado a inserir informações específicas, incluindo um conjunto de perguntas de segurança que foram especificadas ao configurar seu perfil do usuário.

Se você esqueceu seu nome de usuário, entre em contato com o administrador da conta ou com o usuário principal, que tem a capacidade de recuperar seu nome de usuário. Se você for o usuário administrador ou principal na conta, entre em contato com o Suporte para obter assistência adicional.

## O que é o IBMid e como ele se relaciona com os usuários de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_whatisibmid}

Novas contas requerem o IBMid para autenticação. As contas existentes continuam usando o nome de usuário e a senha do SoftLayer para autenticação até que você execute a ferramenta de migração para alternar para um IBMid. Sua conta do SoftLayer tem um usuário principal que tem autoridade para incluir mais usuários dentro dessa mesma conta. Consulte [Como as contas do SoftLayer são gerenciadas no portal do cliente](/docs/customer-portal/cphowacctsman.html) para obter mais informações.

## Como vincular uma conta do SoftLayer existente?
{: #bicp_linkbmxacct}

Se você for o usuário principal em sua conta do SoftLayer, efetue login no portal do cliente e clique em **Vincular uma conta** no cabeçalho.  Veja [Vinculando contas do usuário IBMid](/docs/account/softlayerlink.html) para obter informações adicionais.

## Tenho que ser um usuário existente do {{site.data.keyword.Bluemix_notm}} para vincular contas?
{: #bicp_bmxusertolink}

Não. É possível criar uma nova conta do {{site.data.keyword.Bluemix_notm}} ou vincular uma conta de avaliação ou pré-paga existente do {{site.data.keyword.Bluemix_notm}}.


## Como funciona a autenticação de dois fatores?
{: #bicp_2fa}

Não há nenhum impacto para a configuração de autenticação de dois fatores no nível da conta. A autenticação de dois fatores não é por IBMid; ela ainda é por conta. Quando um IBMid está associado a muitas contas, e você alterna entre as contas, deve-se confirmar sua identidade toda vez que você alterna para uma conta diferente que requer autenticação de dois fatores. Isso é verdadeiro mesmo se a conta anterior e a nova conta são configuradas com o mesmo mecanismo 2FA.

Para obter mais informações sobre o IBMid com a autenticação de dois fatores, consulte [Uso da autenticação de dois fatores em contas vinculadas](/docs/account/softlayerlink.html).


## Quem pode vincular contas?
{: #bicp_wholinkaccts}

Somente usuários principais da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} podem vincular contas do SoftLayer e do {{site.data.keyword.Bluemix_notm}}. O e-mail de um usuário principal também deve estar associado ao proprietário principal da conta do {{site.data.keyword.Bluemix_notm}} que está sendo vinculada.


## O que usarei para efetuar login em cada portal?
{: #bicp_logineachport}

O faturamento de sua conta está vinculado e você pode mover facilmente entre as contas do SoftLayer e do {{site.data.keyword.Bluemix_notm}}, mas as suas identidades de conta permanecem separadas.

* Se sua conta não usar o IBMid para autenticação, continue usando seu ID do SoftLayer para produtos e serviços do SoftLayer e use seu IBMid para produtos e serviços do {{site.data.keyword.Bluemix_notm}}.

* Se sua conta usa o IBMid para autenticação, use seu IBMid para acessar os ambas as contas do SoftLayer e do {{site.data.keyword.Bluemix_notm}}.


## Tentei efetuar login com meu nome de usuário do SoftLayer, por que estou recebendo um erro?
{: #bicp_SLloginerror}

Depois de alternar para um IBMid, se você efetuar login no portal do cliente com seu nome de usuário de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}, verá o erro *"Credenciais de login inválidas fornecidas"*.
Isso ocorre porque, depois de alternar para um IBMid, não é mais possível efetuar login no portal do cliente com seu nome de usuário de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Deve-se clicar em **Login com IBMid** no diálogo de Login da Conta.

## Tentei conectar com meu IBMid, por que estou recebendo um erro?
{: #bicp_IBMidloginerror}

Ao se conectar com seu IBMid, se você receber o erro *"Nós não reconhecemos este IBMid ou e-mail"*, certifique-se de que esteja inserindo um endereço de e-mail completo. Além disso, certifique-se de que não esteja usando seu nome de usuário de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}.


##  Tenho uma nova conta do SoftLayer que usa o IBMid para autenticação; posso usar o mesmo ID para a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} e o {{site.data.keyword.Bluemix_notm}}?
{: #bicp_loginIBMidSLBlusame}

Sim, é possível usar o mesmo IBMid para efetuar login na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} e no {{site.data.keyword.Bluemix_notm}}.


## Eu vinculei uma conta do {{site.data.keyword.Bluemix_notm}}, como posso fornecer acesso aos outros membros da equipe de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_linkgiveteamaccess}

Deve-se convidá-los para o {{site.data.keyword.Bluemix_notm}}. Na interface com o usuário do {{site.data.keyword.Bluemix_notm}}, selecione **Conta e suporte** > **Conta** > **Convidar membros da equipe**. Depois de ter selecionado um grupo de recursos, você verá uma opção para incluir membros da equipe de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Pode ser necessário efetuar login na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} antes de poder enviar convites. O {{site.data.keyword.Bluemix_notm}} obtém a lista de usuários de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} e, em seguida, é possível selecionar quais usuários convidar para a conta do {{site.data.keyword.Bluemix_notm}}.


## Onde está meu e-mail para concluir a comutação para o IBMid?
{: #bicp_ibmidswitchemail}

Se você seguiu o assistente para alternar para o IBMid e não recebeu o e-mail, pode demorar de minutos a horas para que o e-mail com o seu código de registro seja enviado. É possível voltar para a página **Editar perfil do usuário** no portal do cliente e clicar em **Reenviar e-mail** para tentar novamente.


## Terei total acesso raiz à minha conta?
{: #bicp_fullrootaccaccess}

Os usuários principais e aqueles com permissões de administrador têm acesso raiz completo às contas no portal do cliente e à API. Os usuários sem permissões de administrador têm acessibilidade controlada por aqueles com funções de administrador. Essas permissões podem ser atualizadas pelos administradores do portal do cliente [editando um perfil do usuário](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile). Sem permissões de administrador, é possível editar seu perfil do usuário no portal do cliente clicando em seu nome do usuário no painel superior.


## Posso vincular uma conta de assinatura do {{site.data.keyword.Bluemix_notm}}?
{: #bicp_linkbmxsubacct}

Todas as contas vinculadas no {{site.data.keyword.Bluemix_notm}} devem ser contas pré-paga . É possível criar uma nova conta pré-paga ou vincular uma conta existente. Ou, é possível vincular uma conta para teste existente, mas ela será atualizada para uma conta pré-paga.


## Como desvincular minha conta do {{site.data.keyword.Bluemix_notm}} com minha conta de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}?
{: #bicp_unlinkacct}

Após as contas serem vinculadas, elas não podem ser desvinculadas.


## O que é o perfil da minha empresa e onde posso localizá-lo?
{: #bicp_whatfindcompprof}

O perfil da empresa são as informações enviadas no momento da criação da conta e inclui um contato principal para sua empresa, juntamente com o nome da empresa, o endereço e o número de telefone. Essas informações são usadas para uma variedade de razões e devem ser mantidas atuais o tempo todo. Para visualizar o perfil da empresa para sua conta ou para solicitar mudanças, consulte [Atualizando o perfil de sua empresa](/docs/customer-portal/cpmanacctcompprof.html#customerportal_reqcompprofch).

## Onde localizar minhas senhas de dispositivo e software?
{: #bicp_devswpw}

As senhas do dispositivo e de software são armazenadas em dois locais dentro do [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Para recuperar as credenciais do dispositivo, incluindo o nome do usuário raiz ou administrador e a senha para o {{site.data.keyword.baremetal_short}} e o {{site.data.keyword.virtualmachinesshort}}, consulte [Interagir com um dispositivo na visualização de captura instantânea](/docs/vsi/vsi_interact_device_snapshot_view.html). Para visualizar e recuperar rapidamente as credenciais de software que são controladas manualmente usando o portal do cliente, consulte [Gerenciando o acesso ao dispositivo](/docs/vsi/vsi_device_access.html).

## Como manter meus dados da web em sincronia?
{: #bicp_webdatasync}

Embora você seja responsável por manter a consistência de dados entre servidores reais, o {{site.data.keyword.BluSoftlayer_full}} fornece uma rede privada que você pode usar para sincronizar sem incorrer em encargos de uso.


## O que é o Sistema de Gerenciamento de Eventos?
{: #bicp_whatisems}

O Sistema de Gerenciamento de Eventos é um conjunto de ferramentas que otimiza a forma como o {{site.data.keyword.BluSoftlayer_full}} compartilha informações com usuários sobre problemas de infraestrutura não planejados e futuros eventos de manutenção planejados. Ele utiliza alertas de e-mail direcionados baseados em assinatura para esses incidentes para compartilhar o tipo de evento que ocorreu. Ele fornece aos usuários inscritos detalhes adicionais sobre o impacto geral do evento e um status atual do incidente não planejado em andamento (UIP).

## Como e onde posso cancelar um dispositivo?
{: #bicp_candev}

É possível cancelar um dispositivo a qualquer momento por meio do [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}. Consulte [Cancelar um dispositivo](/docs/vsi/vsi_managing.html) para obter mais informações sobre como concluir uma solicitação de cancelamento.
