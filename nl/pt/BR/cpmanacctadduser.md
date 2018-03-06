---

copyright:

  years: 1994, 2018

lastupdated: "2018-02-12"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Incluindo usuários em uma conta do SoftLayer
{: #customerportal_addusertocpacct}

Um ou mais usuários podem interagir com os produtos e serviços associados a uma conta. Se você for o usuário principal, será possível incluir usuários a qualquer momento.
{:shortdesc}

Se você estiver gerenciando usuários de infraestrutura do {{site.data.keyword.BluSoftlayer_full}}, quais contas do SoftLayer poderão ser gerenciadas dependerão do acesso designado à sua conta de usuário e de como sua conta foi configurada. Se você for o usuário principal ou tiver acesso administrativo como um proprietário da conta, será possível gerenciar outros usuários do portal do cliente. Se sua conta não estiver configurada como um usuário principal, será possível gerenciar seu perfil do usuário.

Dependendo de seu acesso, será possível gerenciar sua conta do SoftLayer ou as contas de outros usuários da janela Usuários. A janela Usuários no [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} exibe os usuários associados a uma conta. As interações disponíveis na janela Usuários variam com base em sua permissão de conta exclusiva configurada.
  * Se você for o usuário principal da conta, poderá ver todos os usuários associados à conta.

  Se precisar compartilhar as credenciais de login principal para sua conta, compartilhe as credenciais cuidadosamente. Seu login principal controla cada aspecto de sua conta e deve ser protegido. Para permitir que outros usuários usem o portal do cliente, configure usuários individuais ou baseados em permissões. Isso permite que você tenha maior controle sobre quem é capaz de interagir com determinados aspectos de sua conta.
  {:tip}
  * Se você tiver acesso administrativo, poderá ver todos os usuários que criou e, se você deu permissão a esses usuários para administrar outros usuários, também será possível ver quaisquer usuários que eles criaram. Também é possível executar ações em qualquer usuário associado à conta, incluindo a edição de acesso ao portal do cliente, a mudança de status do usuário e a remoção de usuários.
  * Se você não for o usuário principal da conta e não tiver acesso administrativo, apenas seu perfil será mostrado.  É possível interagir com sua própria conta, inclusive visualizar a chave API, editar o acesso à VPN e incluir autenticação externa.

Para gerenciar usuários do console do {{site.data.keyword.Bluemix_notm}}, consulte a seção [Configuração da conta](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) e [Gerenciando a identidade e o acesso](/docs/iam/quickstart.html#getstarted). Consulte [Como o console do {{site.data.keyword.Bluemix_notm}} funciona](/docs/overview/ui.html#ui) para obter mais informações sobre o console do {{site.data.keyword.Bluemix_notm}}.

Pessoas diferentes em uma organização possuem funções e responsabilidades diferentes e os conjuntos de permissões do usuário não são uniformizados. Portanto, é possível incluir usuários no portal do cliente com funções para assegurar que cada pessoa ou grupo tenha acesso apenas ao que deve. Se forem feitas mudanças com erro ou desautorizadas, será possível rastreá-las de volta até o usuário ou grupo para assegurar que você possa fornecer permissões de treinamento adequado ou de atualização do usuário. Isso minimiza o risco de várias formas e permite que os usuários se concentrem em sua função especificada dentro do portal do cliente.

Use as etapas a seguir para incluir um usuário em uma conta.

1. Acesse o portal do cliente usando suas credenciais exclusivas.
2. Selecione **Conta > Usuários** na barra de navegação.
3. Clique em **Incluir usuário**.
4. Preencha os campos necessários na seção **Informações pessoais**, incluindo o status, um nome de usuário e o endereço de e-mail para comunicação e notificações do portal do cliente, incluindo a notificação inicial para configurar uma senha para a conta.

  Opcionalmente, em vez de inserir um endereço para o usuário, é possível clicar na caixa de seleção **Usar informações da empresa padrão** para preencher o endereço da empresa.
  {: tip}

5. Preencha os campos necessários na seção **Configurações de login**, incluindo se as configurações podem ser editadas pelo usuário, se o endereço IP é restrito e se o usuário precisa ou não configurar e usar perguntas de segurança. Além disso, para quaisquer usuários que não estão usando o IBMid, é possível configurar o período de tempo antes da expiração da senha.
**Notas:**
* Se você usar o IBMid para autenticação, atualize as senhas em seus [perfis do IBMid ![Ícone de link externo](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} seguindo as instruções em **Conectar**.
* Clique na caixa de seleção **Senha do portal do usuário para VPN** para sincronizar as senhas do portal do cliente e da VPN.
6. Clique em **Incluir usuário**.

Após a criação de uma conta para um usuário, o usuário recebe uma notificação por e-mail para concluir a configuração de sua conta configurando uma senha e, opcionalmente, perguntas de segurança se você tiver indicado que elas são necessárias.

Como os usuários sem o acesso administrativo de um usuário principal efetuam login no portal do cliente depende do usuário principal que forneceu o acesso de usuário nas contas do SoftLayer:
  * Se o usuário principal possui um IBMid para autenticar, cada usuário que o usuário principal cria tem um IBMid.
  * Se o usuário principal possui um ID de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para autenticar, cada usuário que o usuário principal cria tem um nome de usuário de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. O usuário principal e cada usuário que o usuário principal cria devem executar a ferramenta de migração para alternar para um IBMid.
  * Se nenhum desses casos se aplicam, no caso de parceiros de negócios IBM por exemplo, entre em contato com o Suporte para determinar qual ID do usuário usar.

## Configurando permissões de usuário na conta
{: #cp_setuserpermsacct}

Use as etapas a seguir para configurar as permissões para o usuário que você acabou de incluir.

1. Clique no ícone **Permissões**, indicado por uma figura de usuário com um bloqueio.
2. Atualize as **Permissões do usuário** em todas as guias para o novo usuário.
> **Nota:** selecione uma opção na lista **Permissões rápidas** para visualizar os conjuntos de permissões recomendados para três tipos de usuários. Clique em **Configurar permissões** para selecionar o conjunto de permissões recomendado ou customize a acessibilidade do usuário selecionando opções individuais em cada guia disponível.
3. Clique em **Incluir permissões do portal** para incluir as permissões ou clique em **Reconfigurar permissões** para reconfigurar permissões para o usuário.
4. Clique no ícone **Acesso ao dispositivo**, indicado por três servidores.
5. Clique na caixa de seleção do dispositivo para cada dispositivo que você deseja que o usuário seja capaz de acessar.
6. Clique em **Atualizar acesso ao dispositivo** depois de selecionar os dispositivos.

Você receberá um e-mail com links e informações para orientá-lo durante a configuração de um IBMid para autenticação nessa conta. As etapas podem incluir criar um novo IBMid se a conta estiver usando o IBMid para autenticação. O convite expira em 7 dias, mas você pode entrar em contato com o administrador para reenviar o convite.

Para todos os outros casos de autenticação, depois de incluir o novo usuário, o usuário pode efetuar login no portal do cliente a qualquer momento para trabalhar com vários produtos e serviços associados à conta. É possível desativar o usuário a qualquer momento.
