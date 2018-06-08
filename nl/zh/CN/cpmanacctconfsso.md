---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-24"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 配置单点登录
{: #customerportal_confssoserv}

如果您是帐户的主用户或具有对帐户的管理访问权，那么可以配置单点登录。为 {{site.data.keyword.BluSoftlayer_full}} 基础架构配置单点登录的过程分为两个步骤。首先，选择并设置身份提供者。然后，设置 {{site.data.keyword.BluSoftlayer_notm}} 基础架构以接收来自身份提供者的认证请求。
{:shortdesc}

## 选择和设置身份提供者
{: #cp_setupidprov}

如果您还没有身份提供者，请先选择身份提供者并对其进行设置。可以将以下身份提供者用于 {{site.data.keyword.BluSoftlayer_notm}}：
* Ping Identity&reg;
* OneLogin&trade;
* IBM&reg; Cloud Security Enforcer
* IBM Cloud Identity Services
有关更多信息，请联系 {{site.data.keyword.BluSoftlayer_notm}} 基础架构销售代表。

如果尚未设置身份提供者，那么可以联系身份提供者支持来获取特定步骤。还可以使用以下高级步骤来配置身份提供者：
1. 通过下载并安装可执行文件来准备身份提供者环境。
2. 配置身份提供者以使用 {{site.data.keyword.BluSoftlayer_notm}} 认证。

## 设置 {{site.data.keyword.BluSoftlayer_notm}} 基础架构进行 SSO
{: #cp_setupsso}

您必须从身份提供者中提取 Security Assertion Markup Language&trade; (SAML&trade;，安全性断言标记语言) 2.0 元数据信息的以下必填字段，以便用于 {{site.data.keyword.BluSoftlayer_notm}}。
<dl>
<dt>实体标识</dt>
<dd>身份提供者的实体标识。</dd>
<dt>单点登录 URL</dt>
<dd>身份提供者用于 SSO 的端点。</dd>
<dt>证书</dt>
<dd>身份提供者用于对请求签名的证书。</dd>
</dl>

以下字段是可选的：
<dl>
<dt>证书指纹</dt>
<dd>证书的指纹。可以使用此字段，而不使用整个证书。</dd>
</dl>

使用以下步骤设置 {{site.data.keyword.BluSoftlayer_notm}} 基础架构以接收来自身份提供者的认证请求：
1. 如果您尚未登录，请登录到身份提供者，并找到 **SAML 配置**页面。请注意以下信息：
  * 实体标识
  * 单点登录 URL
  * 证书（证书需求将根据身份提供者而变化。）
2. 以具有用于创建 SoftLayer 帐户的主用户名和密码的主用户身份登录到 {{site.data.keyword.BluSoftlayer_notm}} 基础架构。
3. 单击**帐户** > **管理** > **SAML 认证**。
4. 输入**身份提供者**元数据。
5. 单击**保存**。
6. 单击**帐户** > **管理** > **SAML 认证**。
7. 单击**下载 XML 配置**以下载服务提供者元数据或记下信息。
8. 使用**服务提供者**元数据以基于身份提供者的指示信息来配置身份提供者。  

您可以使用联合标识登录到 {{site.data.keyword.BluSoftlayer_notm}} 基础架构。有关联合标识的更多信息，请参阅[注册 {{site.data.keyword.Bluemix_notm}}](/docs/account/adminpublic.html) 和 [IBMid Enterprise Federation Adoption Guide ![外部链接图标](../icons/launch-glyph.svg)](https://ibm.box.com/v/IBMid-Federation-Guide){: new_window}。
