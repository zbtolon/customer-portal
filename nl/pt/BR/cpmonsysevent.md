---

copyright:

  years: 1994, 2018

lastupdated: "2018-01-11"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# Monitorando eventos do sistema de infraestrutura do {{site.data.keyword.Bluemix_notm}}
{: #customerportal_monevent}

É possível monitorar eventos do sistema para manter seus sistemas em execução sem problemas.  Para obter informações sobre como configurar e gerenciar servidores virtuais na infraestrutura do {{site.data.keyword.BluSoftlayer_full}}, consulte [Introdução aos servidores virtuais](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers).
{:shortdesc}

## Visualizando um log de auditoria para uma conta
{: #cp_viewacctauditlog}

Cada conta do portal do cliente vem com um log de auditoria que rastreia as interações de cada usuário dentro do portal do cliente. Interações rastreadas incluem tentativas de login (sucesso e falhas), atualizações de velocidade da porta, ligar ou desligar e reinicializar, além daquelas interações feitas pela equipe de suporte de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Use as etapas a seguir para visualizar um log de auditoria para uma conta do usuário.

1. Acesse o [Portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} usando as suas credenciais exclusivas.
2. Selecione **Conta** > **Gerenciar** > **Log de auditoria** na barra de navegação para acessar o log de auditoria.

O log de auditoria inicialmente exibe as últimas 25 interações tomadas por usuários na conta. É possível visualizar até 200 interações a qualquer momento. Atualize o número de resultados mostrados na lista suspensa **Exibir**. Se as configurações mudaram, a coluna **Ação** para a interação conterá um link. Clique em qualquer link para visualizar a configuração impactada pela ação e detalhes sobre a mudança. Clicar no nome de dispositivo ou nome do usuário para qualquer interação redireciona você para a tela de detalhes do dispositivo ou a tela de perfil do usuário, respectivamente.

## Visualizando logs de acesso de um usuário
{: #cp_viewuserlogs}

Logs de acesso exibem dados para cada tentativa de acesso feita por um usuário do portal do cliente específico. Os logs exibem um registro de data e hora e o endereço IP para cada tentativa de acesso. Use as etapas a seguir para visualizar Logs de acesso de um usuário.

1. Acesse o [portal do cliente ![Ícone de link externo](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} usando as suas credenciais exclusivas.
2. Selecione **Conta** > **Usuários** na barra de menus para acessar a janela Usuários.
3. Na lista suspensa **Ações**, selecione **Visualizar log de auditoria** para visualizar o log de acesso do usuário.

O log de acesso para cada usuário exibe as tentativas de acesso feitas por esse usuário por data, juntamente com o endereço IP do qual a tentativa de acesso foi feita. Informações dentro do log de acesso são somente leitura; portanto, as edições para o conteúdo não podem ser feitas a qualquer momento. É possível visualizar os logs de acesso novamente a qualquer momento repetindo as etapas anteriores. Para sair dos logs e retornar à tela Usuários, clique no link **Visualizar todos os usuários**.
