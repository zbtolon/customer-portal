---

copyright:

  years: 1994, 2018

lastupdated: "2018-09-05"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# Assinando as notificações
{: #cp_bpnotifications}

Às vezes, ocorrem eventos na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} que requerem ação; alguns são inesperados e alguns são atividades de manutenção planejadas necessárias para manter a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} operando em sua condição de pico. Os clientes são isolados desses eventos o tanto quanto possível, mas às vezes é necessário colocar o equipamento off-line. Independentemente do impacto para os clientes, é sempre necessário ser transparente, oportuno e informativo.
{:shortdesc}

Como você deve estar no controle de sua experiência de nuvem, são necessárias informações oportunas sobre as atividades de manutenção. Para obter essas informações, é possível assinar notificações do portal do cliente. A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} usa o processo de notificação do Event Management System (EMS) para os tipos de eventos operacionais importantes a seguir:
* Problemas de infraestrutura não planejados: problemas que poderiam causar uma indisponibilidade sob determinadas condições para clientes específicos
* Manutenção de serviço planejada: manutenção que é necessária para manter a infraestrutura operacional no status ideal
* Chamados de suporte abertos: alerta usuários inscritos sobre chamados abertos em suas contas

As notificações de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} foram projetadas para ambientes de nuvem aderindo aos principais princípios a seguir:
* Automatizadas por meio do portal do cliente
* Escaláveis para alcançar uma comunidade grande e crescente
* Destinadas permitindo que a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} identifique apenas os clientes e o subconjunto de recursos afetados pelo evento.

Para que o sistema de notificação seja totalmente eficaz, assine o processo. Se você tiver um ambiente crítico que a requeira, estabeleça também uma cobertura de 24 horas.


## Política de sincronização de notificação
{: #cp_bpgsnotiftimpol}

O período de tempo que a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} fornece aos usuários antecipadamente sobre um evento pendente difere, dependendo de se o evento é um problema de infraestrutura não planejado ou uma manutenção planejada. Geralmente, a política de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} é resolver problemas o mais rápido possível para remover ou minimizar o risco de desenvolver problemas adicionais, o que poderia ter um impacto maior. Isso significa que, às vezes, até mesmo a manutenção planejada é executada com uma curta notificação prévia.

### Visão geral da política
{: #cp_bpgsnotifpolover}

Você será notificado sobre os tipos de interrupções ou problemas a seguir, conforme descrito em cada seção.

#### Problemas ou indisponibilidades não planejados
A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} se comunica com os clientes afetados o mais rápido possível com informações relacionadas ao escopo de infraestrutura, soluções alternativas ou estimativas de resolução assim que essa informação é conhecida. A comunicação oportuna fornece as informações que você precisa para planejar contingências e fornece a garantia de que a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} está tratando a questão.

#### Manutenção planejada
A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} fornece notificação para manutenção planejada antes do evento. Há momentos em que a manutenção da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} é uma emergência, o que pode resultar em notificação prévia mais curta. O objetivo é sempre encontrar o equilíbrio ideal entre dar uma quantidade razoável de notificação prévia para permitir que você planeje contingências e fazer upgrade ou melhorar a infraestrutura, o que normalmente resulta em melhorias na estabilidade geral, ou incluir recursos necessários.

#### Vulnerabilidades de segurança
A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} isola a área afetada, cria uma correção para fechar a vulnerabilidade e testa a correção para assegurar que nenhuma função indireta seja afetada. Geralmente, esse trabalho é feito com outro fornecedor que poderia fornecer partes da tecnologia afetada. Geralmente, há um embargo de notificação pública para correções de segurança, que são mantidas curtas para proteger o público, mas isso exige um período mais curto de notificação prévia. A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} implementa as correções em toda a infraestrutura afetada antes que o público fique ciente do problema, o que de outra forma aumentaria o risco. Quanto mais rápido a vulnerabilidade é encerrada, mais cedo o risco é removido, o que significa que os problemas de segurança requerem uma janela de notificação curta.

Um dos destinos mais frequentes para violações de segurança é o software de infraestrutura virtual. A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} usa software livre popular e tecnologia de parceiro para entregar sua oferta do Virtual Server. Para implementar uma correção de segurança, servidores de cliente que executam software de infraestrutura virtual podem precisar ser colocados off-line para corrigir e reiniciar o ambiente, causando interrupção. Para minimizar o impacto para os clientes, a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} implementou recentemente um aprimoramento no processo de notificação para infraestrutura virtual: comunicações melhoradas. Os clientes são notificados com uma hora de início específica e uma janela de 90 minutos para cada pod, que resulta em um tempo menor de interrupção e em uma sincronização mais precisa para ajudá-los a se preparar melhor. O sistema de notificação isola a manutenção para cada conta, permitindo que a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} notifique os clientes assim que seus hosts específicos são atendidos, o que na maioria das vezes ocorre bem antes da janela de 90 minutos.

#### Vários PODs ou data centers afetados
A infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} se esforça para dar um aviso prévio mais longo, a menos que exista uma urgência extrema para implementar a correção para evitar um impacto secundário ainda maior.


## Incluindo assinantes em notificações de eventos
{: #cp_bpaddsub2eventnotcp}

Cada vez mais, os clientes IBM dependem dos serviços de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} (IaaS), seja contratando a IBM para serviços de infraestrutura gerenciados, contratando para serviços de nuvem que são executados na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} ou contratando diretamente com os serviços de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Quando os serviços de nuvem envolvem infraestrutura, apenas usuários da conta do SoftLayer estão autorizados a receber notificações, conforme descrito na seção anterior. Em alguns casos, é possível que você não deseje que as equipes da Conta IBM ou do Serviço Gerenciado envolvidas nas operações ou no suporte de serviços de infraestrutura acessem suas contas do SoftLayer. Um novo recurso foi incluído no portal do cliente de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} que permite designar uma lista de assinantes, por exemplo a equipe da IBM, para receber notificações sem ter quaisquer privilégios em suas contas.

Para designar uma lista de assinantes, os usuários principais podem efetuar login em suas contas do portal do cliente e usar as etapas a seguir:
1. Clique em  ** Suporte **  >  ** Eventos **  a partir do menu.
2. Escolha o tipo de evento para incluir assinantes.
2. Na janela pop-up, inclua o endereço ou endereços de e-mail. Os endereços de e-mail podem ser IBM ou não IBM.
3. Clique em **Criar**.

Os endereços de e-mail incluídos como assinantes adicionais recebem notificações de eventos planejadas e não planejadas e chamados de suporte abertos. As notificações contêm detalhes técnicos que devem ser considerados ao incluir assinantes. Devido à natureza técnica detalhada das notificações, os assinantes destinados são aqueles que podem entender, em detalhes, como a notificação afeta seu ambiente de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}. Inscrever destinatários que não são capazes de entender o impacto potencial do cliente com base nos detalhes da notificação é contraproducente e altamente desaconselhado.
