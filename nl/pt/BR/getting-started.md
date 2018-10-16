---

copyright:

  years: 1994, 2018

lastupdated: "2018-10-10"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Tutorial Introdução
{: #getting-started}

Nesse tutorial, passaremos pelo processo de introdução e execução com sua conta do SoftLayer para que você possa começar a pedir e gerenciar os recursos de infraestrutura.
{:shortdesc}

## Antes de começar
{: #prereqs}

É necessária uma [conta do {{site.data.keyword.Bluemix}} ![Ícone de link externo](../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net/){:new_window}. Efetue login no portal do cliente com suas credenciais do IBMid. A maioria dos novos usuários usa o [IBMid](/docs/account/softlayerlink.html#switchtoIBMid) para autenticação.

Se você não usa o IBMid para autenticação para efetuar login em sua conta, efetue login no portal do cliente com suas credenciais de infraestrutura exclusivas do {{site.data.keyword.BluSoftlayer_notm}}.
{: tip}

## Etapa 1. Configurar sua conta
{: #account-setup}

A configuração de sua conta inclui a verificação das informações de contato e dos detalhes de faturamento de sua conta:
 * Para verificar os detalhes de contato da empresa, acesse **Conta** > **Gerenciar** > **Contatos da empresa**. As informações de contato da empresa de sua conta são usadas para notificá-lo sobre quaisquer problemas ou mudanças em sua conta.
 * Para verificar os detalhes de perfil de sua empresa, acesse **Conta** > **Gerenciar** > **Perfil da empresa**. As informações de perfil da empresa incluem detalhes sobre o portador da conta principal.
 * Para verificar seus detalhes de faturamento, acesse **Conta** > **Faturamento** > **Método de pagamento**. O método de pagamento mensal é o cartão de crédito faturado em uma base recorrente para os pagamentos associados à sua conta.

## Etapa 2. Incluir os usuários e designar as permissões
{: #users-permissions}

Para incluir usuários em sua conta e configurar permissões iniciais, acesse **Conta** > **Usuários**.
 * Para convidar usuários para ambos os recursos de plataforma e infraestrutura em sua conta com base nas permissões específicas designadas por você, clique em **Convidar usuários**. Em seguida, você é direcionado para a IU do {{site.data.keyword.Bluemix_notm}} Identity and Access Management (Tivoli Information Archive Manager) para convidar usuários e designar acesso. Consulte [Convidando usuários e designando acesso](/docs/iam/iamuserinv.html) para obter mais informações.
 * Para incluir apenas usuários com acesso à VPN, clique em **Incluir usuário somente de VPN**. Insira as informações pessoais, configure as permissões do portal e configure o acesso ao dispositivo para o usuário.

Ao configurar permissões de infraestrutura no convite inicial, você escolhe um de três conjuntos de permissões: Apenas visualização, Usuário básico, Superusuário. Após os usuários aceitarem o convite, é possível customizar seus acessos editando suas permissões do portal. Para obter mais informações, consulte [Infraestrutura Permissões](/docs/iam/infrastructureaccess.html).
{: tip}

## Etapa 3. Ativar o acesso à rede privada da infraestrutura do {{site.data.keyword.Bluemix_notm}}
{: #enable-private-network}

A rede privada de infraestrutura do {{site.data.keyword.Bluemix_notm}} é oferecida para usuários e dispositivos gratuitamente. Toda a largura de banda na rede privada é ilimitada e gratuita. A rede privada oferece os benefícios a seguir:
  * Réplica de ambientes de dispositivo para outros data centers para failover
  * Acessibilidade do sistema front para servidores de banco de dados
  * Acesso e gerenciamento seguros para seus sistemas

Para permitir o acesso de usuário à rede privada, edite o acesso à VPN no portal do cliente:
  1. Selecione **Conta** > **Acesso à VPN** na barra de menus.  
  2. Clique no link na coluna Acesso à VPN.
  3. Selecione uma opção no menu **Tipo de VPN** e clique em **Salvar**.  

Para usuários em contas que usam a autenticação do IBMid, usa-se o nome do usuário da VPN do SoftLayer para acesso à VPN. O nome do usuário da VPN é definido no perfil do usuário e é diferente do nome do usuário padronizado para o endereço de e-mail e ID da conta do IBMid.
{: tip}

Para obter mais informações sobre como usar uma conexão de VPN, veja [Sobre a VPN](/docs/infrastructure/iaas-vpn/about-vpn.html).

## Etapa 4. Assinar notificações
{: #get-notified}

Para ser notificado sobre problemas do sistema que possam ocorrer e eventos de manutenção planejados, é possível assinar notificações por meio do Sistema de Gerenciamento de Eventos. Por padrão, sua assinatura para notificações é cancelada quando você cria uma conta ou é incluído em uma conta.

Acesse o Sistema de gerenciamento de eventos no portal do cliente para especificar quais notificações você deseja assinar:
  1. Selecione **Conta** > **Gerenciar** > **Assinaturas** na barra de menus.
  2. Clique em uma assinatura específica na lista.
  3. Selecione  ** Sim **  na coluna Assinado.
  4. Clique em **Visualizar todas as assinaturas** para retornar à lista de assinaturas disponíveis e assinar outros tipos, se necessário.

## Próximas Etapas
{: #next-steps}

Após sua conta ser configurada, acesse o catálogo do [{{site.data.keyword.Bluemix_notm}} ![Ícone de link externo](../icons/launch-glyph.svg)](https://console.bluemix.net/catalog/?category=infrastructure){:new_window} e comece a pedir dispositivos.
