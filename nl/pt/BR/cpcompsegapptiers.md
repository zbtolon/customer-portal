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

# Protegendo e escalando seu ambiente
{: #cp_compsegapptierssecscal}

Ao hospedar um aplicativo, dois dos aspectos mais críticos a serem considerados por qualquer administrador do sistema são a segurança e a escalabilidade do aplicativo.
{:shortdesc}

## Protegendo seus sistemas com firewalls
{: #cp_bpsecuresystem}

Firewalls são serviços complementares para quaisquer dispositivos que devem ser configurados e ativados manualmente para assegurar que sejam efetivos. É possível bloquear portas supérfluas e desativar portas públicas para sistemas baseados na rede privada para gerenciar ainda mais a acessibilidade externa aos seus sistemas. A execução de varreduras de vulnerabilidade regulares no portal do cliente identifica quaisquer riscos de segurança pendentes ou desconhecidos para que você possa mitigar os riscos rapidamente.

### Ativando seu firewall
{: #cp_bpnofirewalbypass}

Comprar um firewall é o começo para proteger seus sistemas, mas apenas comprar um firewall não protege você. Após ser provisionado, seu firewall está no **Modo Bypass** e não tem regras configuradas. Para que seu firewall funcione, deve-se criar regras e ativar o firewall para que ele possa começar a bloquear atividades indesejadas.


## Protegendo seu ambiente segmentando suas camadas do aplicativo
{: #cp_copmsecenv}

Ao segmentar suas camadas do aplicativo lógico em camadas de infraestrutura física, é possível fornecer maior segurança por meio do uso de listas de controle de acesso (ACLs). Ao segmentar suas camadas do aplicativo, um dos componentes mais críticos a serem considerados é o tráfego permitido em cada camada e sua origem. Para determinar isso, será necessário pensar em como seu aplicativo basicamente funciona e quais serviços dependem uns dos outros para fornecer ao usuário final seu conteúdo solicitado.

Por exemplo, com um aplicativo de duas camadas que depende de uma frente da web e do banco de dados de backend, você precisará assegurar que as portas 80 e 443 (se você estiver usando SSL) estejam abertas à Internet em seus servidores da web. Você provavelmente também deseja bloquear todas as portas para a Internet e gerenciar seu servidor sobre VPN utilizando a rede privada de infraestrutura do {{site.data.keyword.BluSoftlayer_full}}. Nesse cenário, você provavelmente deseja desvincular o endereço IP público em seu servidor de banco de dados e passar todo o tráfego para ele por meio da porta 1433 (para MSSQL) ou da porta 3306 (para {{site.data.keyword.mysql}}) de seu servidor da web.  Seu servidor de banco de dados poderia ser gerenciado pela rede privada, assim como seu servidor da web, e seria possível configurar um firewall de software no servidor de banco de dados para bloquear todo o tráfego do servidor da web para as portas específicas do banco de dados.

Ao configurar seu ambiente dessa maneira, você aumenta a segurança, evitando que as pessoas acessem o SSH ou o RDP da Internet e desativando todo o tráfego de internet para seu banco de dados.  A criação de ACLs entre a camada da web e a camada de banco de dados torna mais difícil comprometer seu banco de dados caso seu servidor da web fique comprometido.

## Escalando seu ambiente segmentando suas camadas do aplicativo
{: #cp_copmscaleenv}

Um ambiente com multicamadas também fornece facilidade de escalabilidade em comparação com arquiteturas de host verticais ou simples. É possível configurar um ambiente com multicamadas para tornar o ajuste de escala de seu aplicativo mais fácil permitindo o ajuste de escala para os serviços que precisam de recursos adicionais. Por exemplo, no cenário anterior, se seu servidor da web está sendo sobrecarregado, é possível simplesmente implementar outro servidor da web, replicar dados do site ou do aplicativo e configurar o balanceamento de carga ou DNS round robin para permitir que seus dois servidores da web dividam sua carga da web. O DNS round robin ou o balanceamento de carga fornece alta disponibilidade para seu ambiente permitindo que vários servidores da web respondam às solicitações recebidas.  Se um único servidor ficar inativo, o outro nó estará disponível para manipular as solicitações do usuário final.

Também é possível escalar seu banco de dados. Por exemplo, com um banco de dados do {{site.data.keyword.mysql}}, uma opção é configurar outro servidor físico e usá-lo como um 'escravo' em uma configuração de replicação Principal/Escravo do {{site.data.keyword.mysql}}.  É possível segmentar todas as suas gravações de banco de dados para o 'principal' e todas as leituras para um ou mais 'escravos' para escalar o banco de dados para suportar mais carga.  Esse tipo de configuração também incluirá um nível de alta disponibilidade permitindo que você mude o status de um 'escravo' para 'principal' e roteie o tráfego de leitura e gravação para ele caso seu nó 'principal' do {{site.data.keyword.mysql}} fique inativo.

Essas ideias são apenas algumas das muitas maneiras de proteger e escalar seu ambiente. Se você tiver perguntas ou interesses relacionados à melhor maneira de arquitetar seu ambiente de uma perspectiva de segurança ou escalabilidade, a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} possui uma equipe de Engenharia de Vendas que poderá ajudar.
