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


# Configurando a conexão única
{: #customerportal_confssoserv}

Se você for o usuário principal de uma conta ou tiver acesso administrativo a ela, será possível configurar a conexão única. A configuração da conexão única para a infraestrutura do {{site.data.keyword.BluSoftlayer_full}} é um processo de duas etapas. Primeiro, você seleciona e configura seu provedor de identidade. Em seguida, você configura a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para receber a solicitação de autenticação de seu provedor de identidade.
{:shortdesc}

## Selecionando e configurando o provedor de identidade
{: #cp_setupidprov}

Se você ainda não tiver um provedor de identidade, primeiro selecione um e configure-o. É possível usar os provedores de identidade a seguir com o {{site.data.keyword.BluSoftlayer_notm}}:
* Ping Identity&reg;,
* OneLogin&trade;,
* IBM&reg; Cloud Security Enforcer,
* IBM Cloud Identity Services.
Entre em contato com seu Representante de Vendas de infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para obter mais informações.

Se você ainda não tiver um provedor de identidade configurado, será possível entrar em contato com o suporte do provedor de identidade para obter etapas específicas. Também é possível usar as etapas de alto nível a seguir para configurar seu provedor de identidade:
1. Prepare o ambiente de seu provedor de identidade fazendo download e instalando o arquivo executável.
2. Configure seu provedor de identidade para funcionar com a autenticação do {{site.data.keyword.BluSoftlayer_notm}}.

## Configurando a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para SSO
{: #cp_setupsso}

Deve-se extrair os campos obrigatórios a seguir das informações de metadados do Security Assertion Markup Language&trade; (SAML&trade;) 2.0 de seu provedor de identidade para usar com o {{site.data.keyword.BluSoftlayer_notm}}.
<dl>
<dt>ID da entidade</dt>
<dd>O ID da entidade do provedor de identidade.</dd>
<dt>URL de conexão única</dt>
<dd>O terminal do provedor de identidade para SSO.</dd>
<dt>Certificado</dt>
<dd>O certificado do provedor de identidade usado para assinar solicitações.</dd>
</dl>

O campo a seguir é opcional:
<dl>
<dt>Impressão digital do certificado</dt>
<dd>A impressão digital do certificado. Esse campo pode ser usado no lugar do certificado inteiro.</dd>
</dl>

Use as etapas a seguir para configurar a infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} para receber a solicitação de autenticação de seu provedor de identidade:
1. Efetue login em seu provedor de identidade, se ainda não estiver conectado, e localize a página **Configuração do SAML**. Anote as informações a seguir:
  * ID da entidade
  * URL de conexão única
  * Certificado (Os requisitos do certificado variam com base em seu provedor de identidade.)
2. Efetue login na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} como o usuário principal com o nome do usuário principal e a senha que você usou para criar sua conta do SoftLayer.
3. Clique em **Conta** > **Gerenciar** > **Autenticação SAML**.
4. Insira os metadados do **Provedor de identidade**.
5. Clique em **Salvar**.
6. Clique em **Conta** > **Gerenciar** > **Autenticação SAML**.
7. Clique em **Fazer download da configuração XML** para fazer download dos metadados do provedor de serviços ou anote as informações.
8. Use os metadados do **Provedor de serviços** para configurar seu provedor de identidade com base nas instruções de seu provedor de identidade.  

É possível efetuar login na infraestrutura do {{site.data.keyword.BluSoftlayer_notm}} usando seu ID federado. Para obter mais informações sobre IDs federados, consulte [Inscrevendo-se para o {{site.data.keyword.Bluemix_notm}}](/docs/account/adminpublic.html) e [IBMid Enterprise Federation Adoption Guide ![Ícone de link externo](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}.
