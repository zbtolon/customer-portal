---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-22"

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

Se você estiver gerenciando os usuários da infraestrutura do {{site.data.keyword.BluSoftlayer_full}}, as contas do SoftLayer que você poderá gerenciar dependem do acesso designado à sua conta de usuário. As contas que você pode gerenciar também dependem de como sua conta foi configurada. Se você for o usuário principal ou tiver acesso administrativo como um proprietário da conta, será possível gerenciar outros usuários do portal do cliente. Se sua conta não estiver configurada como um usuário principal, será possível gerenciar seu perfil do usuário.

Dependendo de seu acesso, será possível gerenciar sua conta do SoftLayer ou as contas de outros usuários da janela Usuários. A janela Usuários no [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} exibe os usuários associados a uma conta. As interações que estão disponíveis na janela Usuários variam com base em sua permissão de conta exclusiva configurada.
  * Se você for o usuário principal da conta, poderá ver todos os usuários associados à conta.

  Se precisar compartilhar as credenciais de login principal para sua conta, compartilhe as credenciais cuidadosamente. Seu login principal controla cada aspecto de sua conta; proteja-o cuidadosamente. Para permitir que outros usuários usem o portal do cliente, configure usuários individuais ou baseados em permissões. A criação de usuários baseados em permissão assegura que você tenha maior controle sobre quem é capaz de interagir com determinados aspectos de sua conta.
{:tip}

  * Se você tiver acesso administrativo, será possível ver todos os usuários incluídos. Se tiver dado a esses usuários permissões para administrar outros usuários, também será possível ver quaisquer usuários incluídos. Também será possível gerenciar qualquer usuário que estiver associado à conta, incluindo a edição de acesso ao portal do cliente, a mudança de status do usuário e a remoção de usuários.
  * Se você não for o usuário principal da conta e não tiver acesso administrativo, apenas seu perfil será mostrado. É possível interagir com sua própria conta, inclusive visualizar a chave API, editar o acesso à VPN e incluir autenticação externa.

Para gerenciar usuários do console do {{site.data.keyword.Bluemix_notm}}, consulte a seção [Configuração da conta](/docs/account/adminpublic.html#signing-up-for-ibm-cloud) e [Gerenciando a identidade e o acesso](/docs/iam/quickstart.html#getstarted). Para obter mais informações sobre o console do {{site.data.keyword.Bluemix_notm}}, veja [Como o console do {{site.data.keyword.Bluemix_notm}} funciona](/docs/overview/ui.html#ui).

Pessoas diferentes em uma organização possuem funções e responsabilidades diferentes e os conjuntos de permissões do usuário não são uniformizados. Portanto, é possível incluir usuários no portal do cliente com funções para fornecer acesso a exatamente o que eles precisam para sua função específica. Se forem feitas mudanças por engano ou sem autorização, será possível rastreá-las de volta para o usuário ou o grupo. Portanto, é possível fornecer treinamento adequado ou atualizar a permissão do usuário para minimizar o risco. Seus usuários poderão então se concentrar em sua função especificada dentro do portal do cliente.

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

Depois que você criar uma conta para um usuário, ele receberá uma notificação por e-mail para concluir a configuração de sua conta. O usuário deverá configurar uma senha e, opcionalmente, criar perguntas de segurança se você tiver indicado a necessidade delas.

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
5. Clique na caixa de seleção do dispositivo para cada dispositivo que você deseja que o usuário seja capaz de acessar.
6. Clique em **Atualizar acesso ao dispositivo** depois de selecionar os dispositivos.

Você recebe um e-mail com links e informações para orientá-lo durante a configuração de um IBMid para autenticação nessa conta. As etapas podem incluir criar um novo IBMid se a conta estiver usando o IBMid para autenticação. O convite expira em 7 dias, mas você pode entrar em contato com o administrador para reenviar o convite.

Para todos os outros casos de autenticação, depois de incluir o novo usuário, o usuário poderá então efetuar login no portal do cliente a qualquer momento. Os usuários poderão, assim, trabalhar com vários produtos e serviços associados à conta. É possível desativar o usuário a qualquer momento.
