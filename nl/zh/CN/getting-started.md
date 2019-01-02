---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 入门教程
{: #getting-started}

在本教程中，我们将逐步指导您完成启动并运行 SoftLayer 帐户的过程，以便您可以开始订购和管理基础架构资源。
{:shortdesc}

## 开始之前
{: #prereqs}

您需要 [{{site.data.keyword.Bluemix}} 帐户 ![外部链接图标](../icons/launch-glyph.svg "外部链接图标")](https://cloud.ibm.com){:new_window}。使用您的 IBM 标识凭证登录到客户门户网站。大部分新用户使用 [IBM 标识](/docs/account/softlayerlink.html#switchtoIBMid)进行认证。

如果不使用 IBM 标识进行认证以登录帐户，请使用唯一的 {{site.data.keyword.BluSoftlayer_notm}} 基础架构凭证登录到客户门户网站。
{: tip}

## 步骤 1. 设置帐户
{: #account-setup}

设置您的帐户包括验证帐户联系人信息和记帐详细信息：
 * 要验证公司联系人详细信息，请转至**帐户** > **管理** > **公司联系人**。您帐户的公司联系人信息用于通知您有关帐户的任何问题或更改。
 * 要验证公司概要文件详细信息，请转至**帐户** > **管理** > **公司概要文件**。公司概要文件信息包含有关主帐户持有者的详细信息。
 * 要验证记帐详细信息，请转至**帐户** > **记帐** > **付款方式**。每月付款方式是针对与您帐户关联的付款对信用卡进行周期性记帐。

## 步骤 2. 添加用户和分配许可权
{: #users-permissions}

要将用户添加到您的帐户并设置初始许可权，请转至**帐户** > **用户**。
 * 要根据您分配的特定许可权来邀请用户访问您帐户中的平台和基础架构资源，请单击**邀请用户**。然后，系统会将您定向到 {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) UI 以邀请用户并分配访问权。有关更多信息，请参阅[邀请用户](/docs/iam/iamuserinv.html)。

 * 要添加仅具有 VPN 访问权的用户，请单击**添加仅使用 VPN 的用户**。输入个人信息，设置门户网站许可权，并为用户设置设备访问权。

在初始邀请中设置基础架构许可权时，可以选择以下三个许可权集之一：仅查看、基本用户和超级用户。用户接受邀请后，可以通过编辑其门户网站许可权来定制其访问权。有关更多信息，请参阅[基础架构许可权](/docs/iam/infrastructureaccess.html)。
{: tip}

## 步骤 3. 启用对 {{site.data.keyword.Bluemix_notm}} 基础架构专用网络的访问
{: #enable-private-network}

{{site.data.keyword.Bluemix_notm}} 基础架构专用网络免费向用户和设备提供。专用网络上的所有带宽均不限流量且免费。专用网络的优点众多，包括：
  * 将设备环境复制到其他数据中心以进行故障转移
  * 针对数据库服务器的前端系统可访问性
  * 确保系统访问和管理的安全

要启用用户对专用网络的访问权，请在客户门户网站中编辑 VPN 访问：
  1. 从菜单栏中选择**帐户** > **VPN 访问**。  
  2. 单击“VPN 访问”列中的链接。
  3. 从 **VPN 类型**菜单中选择一个选项，然后单击**保存**。  

对于帐户中使用 IBM 标识进行认证的用户，将使用 SoftLayer VPN 用户名进行 VPN 访问。VPN 用户名在用户概要文件中进行定义。VPN 用户名与缺省为 IBM 标识电子邮件地址和帐户标识的用户名不同。
{: tip}

有关使用 VPN 连接的更多信息，请参阅[关于 VPN](/docs/infrastructure/iaas-vpn/about-vpn.html)。

## 步骤 4. 预订通知
{: #get-notified}

要获得有关系统问题和计划维护事件的通知，您可以通过事件管理系统预订通知。您创建帐户时或者将您添加到帐户时，缺省情况下您未预订通知。

访问客户门户网站中的事件管理系统，以选择要预订的通知：

  1. 从菜单栏中选择**帐户** > **管理** > **预订**。
  2. 单击列表中的特定预订。
  3. 选中“已预订”列中的**是**。
  4. 单击**查看所有预订**以返回可用预订列表，并根据需要预订其他类型。

## 后续步骤
{: #next-steps}

设置帐户后，请转至 [{{site.data.keyword.Bluemix_notm}}“目录”![外部链接图标](../icons/launch-glyph.svg)](https://{DomainName}/catalog/?category=infrastructure){:new_window}，然后开始订购设备。
