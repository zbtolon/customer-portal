---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Incluindo usuários em uma conta do SoftLayer
{: #customerportal_addusertocpacct}

Um ou mais usuários podem interagir com os produtos e serviços associados a uma conta. Se você for o usuário principal ou se tiver acesso administrativo, será possível incluir usuários.
{:shortdesc}

Se você estiver gerenciando usuários da infraestrutura do {{site.data.keyword.BluSoftlayer_full}}, as contas do SoftLayer que poderão ser gerenciadas dependerão do acesso designado à sua conta de usuário. As contas que você pode gerenciar também dependem de como sua conta foi configurada. Se você for o usuário principal ou tiver acesso administrativo como um proprietário da conta, será possível gerenciar outros usuários do portal do cliente. Se a sua conta não estiver configurada como um usuário principal, será possível gerenciar seu perfil de usuário.

Dependendo de seu acesso, será possível gerenciar sua conta do SoftLayer ou as contas de outros usuários da janela Usuários. A janela Usuários no [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} exibe os usuários associados a uma conta. As interações que estão disponíveis na janela Usuários variam com base em sua permissão de conta exclusiva configurada.
  * Se for o usuário principal da conta, será possível ver todos os usuários associados a ela.

  Se precisar compartilhar as credenciais de login principal para sua conta, compartilhe as credenciais cuidadosamente. Seu login principal controla cada aspecto de sua conta. deve-se protegê-lo cuidadosamente. Para permitir que outros usuários usem o portal do cliente, configure usuários individuais ou baseados em permissões. A criação de usuários com base em permissões assegura que você tenha o maior controle sobre quem pode interagir com determinados aspectos de sua conta.
{:tip}

  * Se você tiver acesso administrativo, será possível ver todos os usuários incluídos. Se tiver dado a esses usuários permissões para administrar outros usuários, também será possível ver quaisquer usuários incluídos. Também é possível gerenciar qualquer usuário que esteja associado à conta. Isso inclui editar o acesso ao portal do cliente, mudar o status do usuário e remover usuários.

Para gerenciar usuários do console do {{site.data.keyword.Bluemix_notm}}, consulte a seção [Configuração da conta](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) e [Gerenciando a identidade e o acesso](/docs/iam/quickstart.html#getstarted). Para obter mais informações sobre o console do {{site.data.keyword.Bluemix_notm}}, consulte [Navegando no console do {{site.data.keyword.Bluemix_notm}}](/docs/overview/ui.html#ui).

Pessoas diferentes dentro de uma organização têm diferentes funções e responsabilidades e os conjuntos de permissões do usuário não são de tamanho único. É possível incluir usuários no portal do cliente com funções para fornecer acesso a exatamente o que eles precisam para sua função específica. Se forem feitas mudanças por engano ou sem autorização, será possível rastreá-las de volta para o usuário ou o grupo. Portanto, é possível fornecer treinamento adequado ou atualizar a permissão do usuário para minimizar o risco. Seus usuários poderão então se concentrar em sua função especificada dentro do portal do cliente.

Use as etapas a seguir para incluir um usuário em uma conta.

1. Acesse o portal do cliente usando as suas credenciais exclusivas.
2. Selecione **Conta > Usuários** na barra de navegação.
3. Clique em **Incluir usuário**.
4. Preencha os campos obrigatórios na seção **Informações pessoais**. Forneça o status, um nome de usuário e o endereço de e-mail para comunicação e notificações do portal do cliente, incluindo a notificação inicial para configurar uma senha para a conta.

  Opcionalmente, em vez de inserir um endereço para o usuário, é possível clicar na caixa de seleção **Usar informações da empresa padrão** para preencher o endereço da empresa.
  {: tip}

5. Preencha os campos obrigatórios na seção **Configurações de login**. Especifique se as configurações poderão ser editadas pelo usuário, se o endereço IP será restrito e se o usuário precisará configurar e usar perguntas de segurança. Além disso, para quaisquer usuários que não estão usando o IBMid, é possível configurar o período de tempo antes da expiração da senha.
**Notas:**
* Se você usar o IBMid para autenticação, atualize as senhas em seus [perfis do IBMid ![Ícone de link externo](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} seguindo as instruções em **Conectar**.
* Clique na caixa de seleção **Usar senha do portal para VPN** para sincronizar as senhas do portal do cliente e da VPN.
6. Clique em **Incluir usuário**.

Depois que você criar uma conta para um usuário, ele receberá uma notificação por e-mail para concluir a configuração de sua conta. O usuário deve configurar uma senha e, opcionalmente, criar perguntas de segurança, no caso de você indicar que elas são necessárias.

Como os usuários sem o acesso administrativo de um usuário principal efetuam login no portal do cliente depende do usuário principal que forneceu o acesso de usuário nas contas do SoftLayer:
  * Se o usuário principal possui um IBMid para autenticar, cada usuário que o usuário principal cria tem um IBMid.
  * Se o usuário principal possui um ID de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para autenticar, cada usuário que o usuário principal cria tem um nome de usuário de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. O usuário principal e cada usuário que o usuário principal cria devem executar a ferramenta de migração para alternar para um IBMid.
  * Se nenhum desses casos se aplicar, para Parceiros de Negócios IBM por exemplo, entre em contato com o Suporte para determinar qual ID do usuário usar.

## Configurando permissões de usuário na conta
{: #cp_setuserpermsacct}

Use as etapas a seguir para configurar as permissões para o usuário que você acabou de incluir.

1. Clique no ícone **Permissões**, indicado por uma figura de usuário com um bloqueio.
2. Atualize as **Permissões do usuário** em todas as guias para o novo usuário.
> **Nota:** selecione uma opção na lista **Permissões rápidas** para visualizar os conjuntos de permissões para três tipos de usuários. Clique em **Configurar permissões** para selecionar o conjunto de permissões ou customize a acessibilidade do usuário selecionando opções individuais em cada guia disponível.
3. Clique em **Incluir permissões do portal** para incluir as permissões ou clique em **Reconfigurar permissões** para reconfigurar permissões para o usuário.
4. Clique no ícone **Acesso ao dispositivo**, indicado por três servidores.
5. Clique na caixa de seleção de cada dispositivo que você deseja que o usuário acesse.
6. Clique em **Atualizar acesso ao dispositivo** depois de selecionar os dispositivos.

Você recebe um e-mail com links e informações para orientá-lo durante a configuração de um IBMid para autenticação nessa conta. As etapas podem incluir criar um novo IBMid se a conta estiver usando o IBMid para autenticação. O convite expira em 7 dias, mas você pode entrar em contato com o administrador para reenviar o convite.

Para todos os outros casos de autenticação, depois de incluir o novo usuário, ele poderá efetuar login no portal do cliente a qualquer momento. Os usuários podem trabalhar com vários produtos e serviços associados à conta. É possível desativar o usuário a qualquer momento.
