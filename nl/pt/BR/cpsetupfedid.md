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

# Configurando a federação de identidade
{: #cp_setupidfed}

É possível configurar a federação de identidade para ativar um provedor de serviços, como o {{site.data.keyword.BluSoftlayer_full}} Infrastructure Management System (IMS), para consumir tokens de segurança gerados em um sistema de identidade confiável para propósitos de autenticação e autorização.
{:shortdesc}

É possível configurar a federação de identidade na SSO da infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} de uma das maneiras a seguir:
* Criando usuários no provedor de identidade e na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}
* Criando usuários no provedor de identidade

Uma função define, para o provedor de serviços, o que o usuário está autorizado a fazer (por meio de permissões) em seu sistema depois que o usuário foi autenticado. Por exemplo, a função *Usuário* pode ter permissão apenas para visualizar telas diferentes, mas não para atualizar ou incluir.

Múltiplos usuários podem ser designados a uma única função. Além disso, se uma função existir no provedor de identidade, mas não na infraestrutura do {{site.data.keyword.BluSoftlayer}}, o usuário ainda poderá efetuar login na infraestrutura do {{site.data.keyword.BluSoftlayer}}, mas o usuário não terá nenhuma permissão designada a uma função.
{: tip}


## Criando usuários no provedor de identidade e na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}
{: #cp_scenario1both}

Nesse modelo, ocorre o seguinte:
* Os usuários são criados no provedor de identidade e na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}.
* As permissões de usuário são designadas no IMS da infraestrutura do {{site.data.keyword.BluSoftlayer}} usando o portal do cliente de infraestrutura do {{site.data.keyword.BluSoftlayer}} ou as APIs.
* Os usuários se autenticam no provedor de identidade e federam suas credenciais.
* A infraestrutura do {{site.data.keyword.BluSoftlayer}} consome as credenciais e o controle de acesso baseia-se nas permissões definidas para o usuário no IMS da infraestrutura do {{site.data.keyword.BluSoftlayer}}.

Contas para usuários que precisam de acesso à infraestrutura do {{site.data.keyword.BluSoftlayer}} são criadas primeiro na infraestrutura do {{site.data.keyword.BluSoftlayer}} com senhas aleatórias. Todas as permissões devem ser configuradas na infraestrutura do {{site.data.keyword.BluSoftlayer}} antes de o usuário ser capaz de usar a SSO por meio do provedor de identidade. Atualmente, as permissões são configuradas com base no usuário individual.

### Configurando um usuário
Use as etapas a seguir para configurar um usuário:

1. [Crie usuários na infraestrutura do {{site.data.keyword.BluSoftlayer}}](/docs/customer-portal/cpmanacctadduser.html#customerportal_addusertocpacct).
2. Designe permissões na infraestrutura do {{site.data.keyword.BluSoftlayer}}.
3. Crie usuários no provedor de identidade.

O campo **E-mail** ou **Nome de usuário** dentro do perfil do usuário individual é usado para o token Security Assertion Markup Language&trade; (SAML&trade;) 2.0, que mapeia usuários entre o provedor de identidade e a infraestrutura do {{site.data.keyword.BluSoftlayer}}.

### Exemplo de fluxo para autenticação de login
A seguir há um fluxo de exemplo de como a autenticação de login do usuário pode funcionar ao criar usuários no provedor de identidade e na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}}:
1. O usuário acessa a URL do provedor de identidade de uma sessão do navegador.
2. O provedor de identidade autentica o usuário, por exemplo, através de seu LDAP.
3. O provedor de identidade retorna respostas do SAML 2.0.
4. O provedor de identidade envia uma resposta SAML 2.0 para o provedor de serviços, neste caso a infraestrutura do {{site.data.keyword.BluSoftlayer}}, para autenticar o ID do usuário.
5. A infraestrutura do {{site.data.keyword.BluSoftlayer}} valida a resposta do SAML 2.0.
6. O usuário efetuou login no portal do cliente de infraestrutura do {{site.data.keyword.BluSoftlayer}} com base na configuração confiável entre o provedor de identidade e a infraestrutura do {{site.data.keyword.BluSoftlayer}}.


## Criando usuários no provedor de identidade
{: #cp_scenario2idp}

Nesse modelo, as coisas acontecem conforme a seguir:
* As funções são criadas no provedor de identidade e designadas ao usuário.
* As designações de função e permissão são configuradas no IMS da infraestrutura do {{site.data.keyword.BluSoftlayer}} usando APIs de infraestrutura do {{site.data.keyword.BluSoftlayer}}.
* Os usuários se autenticam no provedor de identidade e federam suas credenciais e atributos de função.
* A infraestrutura do {{site.data.keyword.BluSoftlayer}} consome as credenciais do usuário e os atributos de função. Se a função designada pelo provedor de identidade do usuário corresponder à função na infraestrutura do {{site.data.keyword.BluSoftlayer}}, o usuário receberá as permissões para essa função ao efetuar login na infraestrutura do {{site.data.keyword.BluSoftlayer}}.
* Os usuários criados no provedor de identidade são considerados federados porque eles, e suas funções, são autenticados por meio do SAML 2.0.

### Configurando uma função para um usuário
Use as etapas a seguir para configurar uma função para um usuário:

1. Configure funções por meio da API de infraestrutura do {{site.data.keyword.BluSoftlayer}}.
2. Configure funções no provedor de identidade.
3. Assegure-se de que as funções definidas na infraestrutura do {{site.data.keyword.BluSoftlayer}} e no provedor de identidade tenham o mesmo nome.

### Configurando um usuário
{: #setupuser}

Use as etapas a seguir para configurar um usuário:

1. Configure os usuários no provedor de identidade.
2. Designe funções aos usuários no provedor de identidade.

Nesse cenário, não há necessidade de criar usuários manualmente na infraestrutura do {{site.data.keyword.BluSoftlayer}}.

### Exemplo de fluxo para autenticação de login do usuário
A seguir há um fluxo de exemplo de como a autenticação de login do usuário pode funcionar ao criar usuários no provedor de identidade:
1. O usuário acessa a URL do provedor de identidade de uma sessão do navegador.
2. O provedor de identidade autentica o usuário, por exemplo, através de seu LDAP.
3. O provedor de identidade retorna respostas do SAML 2.0.
4. O provedor de identidade envia uma resposta SAML 2.0 para o provedor de serviços, neste caso a infraestrutura do {{site.data.keyword.BluSoftlayer}}, para autenticar a função de usuário.
5. A infraestrutura do {{site.data.keyword.BluSoftlayer}} valida a resposta do SAML 2.0.
6. A infraestrutura do {{site.data.keyword.BluSoftlayer}} redireciona o usuário para o portal do cliente.
7. O usuário efetuou login no portal do cliente de infraestrutura do {{site.data.keyword.BluSoftlayer}}.

Revise os procedimentos de seu provedor de identidade para configurar novas funções e como associá-las à infraestrutura do {{site.data.keyword.BluSoftlayer}}.
