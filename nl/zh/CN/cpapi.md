---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-19"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# SoftLayer API
{: #customerportal_api}

您可以通过在开发环境中使用直接 API 调用（而不使用客户门户网站），从而使用此 API 与您的帐户、产品和服务进行交互。
{:shortdesc}

此 API 的目标是提供一个环境，在其中可以完成该 API 中的任何客户门户网站任务。API 环境通过经常新增功能和更新进行维护，以确保您可以使用最佳选项。这包括能够使用各种语言进行编程，还可以选择使用 SOAP、XML-RPC 和基于 REST 的 API。与在客户门户网站中工作类似，如果您主要在 API 中进行帐户交互，那么也需要一个可行的支持来源。

## 如何访问 API？
{: #cp_getapikey}

您可以使用特定于用户的 API 密钥访问 API。API 密钥是唯一的字母数字标识，允许您安全访问 API。您的 API 密钥专门链接到您的用户标识，并且在 API 中提供的许可权与您在客户门户网站中所拥有的许可权相同。只需生成 API 密钥一次，然后可以检索该密钥并继续使用。使用以下步骤生成 API 密钥：

1. 使用您的唯一凭证来访问客户门户网站。
2. 从导航栏中选择**帐户** > **用户**。
3. 在具有用户凭证的行的 **API 密钥**列下，单击**生成**链接。

生成 API 密钥之后，**生成**链接会更改为**查看**链接，可随时用于访问您的 API 密钥。

## 在哪里可以了解有关此 API 的更多信息？
{: #cp_apimoreinfo}

[SoftLayer 开发网络 (SLDN) ![外部链接图标](../icons/launch-glyph.svg)](http://sldn.softlayer.com/){:new_window} 致力于在您使用此 API 与帐户、产品和服务进行交互时为您提供支持。[SLDN ![外部链接图标](../icons/launch-glyph.svg)](http://sldn.softlayer.com/){:new_window} 包含有关 SoftLayer API、支持的编程语言、可用的 API 调用等的文档。SLDN 是一种资源，用于获取各种 API 功能相关信息、完整 API 调用列表以及各种博客帖子，让您了解如何最好地使用此 API。


如果您对 API 有任何疑问，可以将问题发布到客户论坛或直接通过文章进行反馈。
