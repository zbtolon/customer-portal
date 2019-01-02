---

copyright:

  years: 1994, 2018

lastupdated: "2018-10-11"

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

Use os firewalls de hardware disponíveis para assegurar que seu dispositivo esteja sempre seguro. É possível provisionar firewalls de hardware sob demanda sem tempo de inatividade, se as regras estiverem estabelecidas corretamente, para proteger seu servidor contra atividade indesejada.

Firewalls são serviços complementares para quaisquer dispositivos que devem ser configurados e ativados manualmente para assegurar que sejam efetivos. É possível bloquear portas supérfluas e desativar portas públicas para sistemas baseados na rede privada para gerenciar ainda mais a acessibilidade externa aos seus sistemas. Varreduras de vulnerabilidade regulares no portal do cliente identificam quaisquer riscos pendentes ou desconhecidos para que seja possível reduzir os riscos rapidamente.

Depois de pedir o firewall, ele deve ser ativado e as regras devem ser configuradas.

### Ativando seu firewall
{: #cp_bpnofirewalbypass}

A compra de um firewall é um começo para proteger seus sistemas, mas a simples compra de um firewall não protege você. Depois de ser provisionado, seu firewall está no **Modo bypass** e não tem regras configuradas. Para que seu firewall funcione, deve-se criar regras e ativar o firewall para que ele possa começar a bloquear atividades indesejadas.


## Protegendo seu ambiente segmentando suas camadas do aplicativo
{: #cp_copmsecenv}

Ao segmentar suas camadas de aplicativo lógicas em camadas de infraestrutura físicas, é possível fornecer maior segurança usando as listas de controle de acesso (ACLs). Ao segmentar suas camadas de aplicativo, um dos componentes mais críticos a serem considerados é o tráfego permitido em cada camada e de onde ele vem. Para determinar essas informações, pense em como seu aplicativo funciona basicamente e que serviços confiam um no outro para fornecer aos usuários o conteúdo solicitado.

Por exemplo, considere um aplicativo de duas camadas que conte com um web front e um backend de banco de dados. Para esse aplicativo, assegure-se de que as portas 80 e 443 (se estiver usando SSL) estejam abertas à internet em seus servidores da web. Provavelmente você também desejará bloquear todas as portas para a internet e gerenciar seu servidor pela VPN usando a rede privada da infraestrutura do {{site.data.keyword.BluSoftlayer_full}}. Você também desejará provavelmente desvincular o endereço IP público em seu servidor de banco de dados e passar todo o tráfego para ele pela porta 1433 (para MSSQL) ou pela porta 3306 (para {{site.data.keyword.mysql}}) por meio de seu servidor da web. Você pode gerenciar seu servidor de banco de dados pela rede privada assim como seu servidor da web. Também será possível configurar um firewall de software no servidor de banco de dados para bloquear todo o tráfego do servidor da web para as portas do banco de dados específicas.

Ao configurar seu ambiente dessa forma, impedindo o acesso ao SSH ou ao RDP pela internet e desativando todo o tráfego de internet para seu banco de dados, você aumenta a segurança. Criar ACLs entre sua camada da web e a camada do banco de dados tornará mais difícil comprometer seu banco de dados se seu servidor da web estiver comprometido.

## Escalando seu ambiente segmentando suas camadas do aplicativo
{: #cp_copmscaleenv}

Um ambiente com multicamadas também fornece facilidade de escalabilidade em comparação com arquiteturas de host verticais ou simples. É possível configurar um ambiente com multicamadas para tornar a ampliação de escala de seu aplicativo mais fácil permitindo o ajuste de escala para os serviços que precisam de mais recursos. Por exemplo, no cenário anterior, se seu servidor da web estiver sendo muito tributado, será possível implementar outro servidor da web. Será possível então replicar os dados do site ou do aplicativo e equilibrar a carga ou configurar o DNS de round robin para permitir que seus dois servidores da web dividam sua carga da web. O DNS de round robin ou o equilíbrio da carga fornece alta disponibilidade para seu ambiente permitindo que os diversos servidores da web respondam a solicitações recebidas. Se um único servidor ficar inativo, outro nó estará disponível para manipular suas solicitações de usuários.

Também é possível escalar seu banco de dados. Por exemplo, com um banco de dados do {{site.data.keyword.mysql}}, uma opção é configurar outro servidor físico e usá-lo como um subordinado em uma configuração de replicação do {{site.data.keyword.mysql}}. É possível segmentar todas as suas gravações de banco de dados para o principal e todas as leituras para um ou mais subordinados a fim de ampliar a escala do banco de dados para suportar mais carga. Esse tipo de instalação também inclui um nível de alta disponibilidade, porque é possível mudar o status de um subordinado para principal. Será possível então rotear tanto o tráfego de leitura quanto o de gravação para o subordinado se seu nó principal do {{site.data.keyword.mysql}} ficar inativo.

Essas ideias são apenas algumas das muitas maneiras de proteger e escalar seu ambiente. Caso você tenha quaisquer perguntas ou dúvidas relacionadas à melhor forma de projetar seu ambiente de uma perspectiva de segurança ou escalabilidade, a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} tem uma equipe de Engenharia de vendas que pode ajudar.
