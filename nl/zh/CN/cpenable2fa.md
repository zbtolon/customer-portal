---

copyright:

  years: 2018

lastupdated: "2018-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 设置双因子认证
{: #customerportal_2fa}

在客户门户网站中，可以激活外部双因子认证 (2FA)，以在登录到门户网站时提供额外的保护。这个额外的安全层可保护帐户免受未经验证的访问，确保设备、数据和帐户信息安全可靠。
{:shortdesc}

如果在客户门户网站为现有 SoftLayer 帐户启用了 2FA，那么会要求您在登录到 {{site.data.keyword.Bluemix_notm}} 控制台时输入安全代码。2FA 仅适用于 {{site.data.keyword.Bluemix_notm}} 帐户中的基础架构资源。无需完成 2FA，就可以对 {{site.data.keyword.Bluemix_notm}} 帐户中的资源执行各种操作。

SoftLayer 帐户的 2FA 不是按 IBM 标识启用的。而是仍按帐户启用。如果一个 IBM 标识与多个帐户相关联，而您会切换不同的帐户，那么每次切换到不同帐户时，都必须确认身份。在帐户之间切换时，您必须确认身份，即使旧帐户和新帐户都配置了相同的 2FA 机制，也是如此。

## 启用 2FA

2FA 认证有两种形式。可以为每个用户同时添加这两种外部认证方法，每月只需支付少量费用：

* Symantec Identify Protection 是最常用的外部认证工具，会要求您在访问客户门户网站时，除了提供用户名和密码外，还使用它提供的动态安全代码。
* PhoneFactor 认证是通过电话呼叫、短信或移动应用程序提供带外认证。

 如果您拥有链接的帐户，那么可以对整个 {{site.data.keyword.Bluemix_notm}} 帐户[启用多因子认证](/docs/iam/mfa.html)，从而利用多因子认证 (MFA) 设置。
 {: tip}

要设置 2FA，请完成以下步骤：

1. 在客户门户网站中，访问**用户**屏幕。
2. 从用户的**操作**菜单中，选择**添加外部认证**。
3. 根据要订购的外部认证的类型，完成以下步骤：
    * 如果选择 Symantec Identity Protection，请选择 **Symantec Identity Protection**，然后输入用户的凭证标识。
    * 如果选择 PhoneFactor，请选择 **PhoneFactor**。
4. 单击**继续**。
5. 在屏幕上完成提供**促销代码**和 **MSA 确认**的提示。
6. 单击**订购外部认证**以完成订单。单击**取消**可取消操作。

## 后续步骤
{: #2fanextsteps}

为用户添加外部认证后，后续步骤取决于认证类型。
* 如果启用了 Symantec Identity Protection，那么必须添加与用户的凭证标识关联的安全代码。此安全代码是在将 Symantec Identity Protection 添加到帐户时，在系统中输入的代码。
* 如果启用了 PhoneFactor，那么用户必须激活 PhoneFactor 才能将此类型的双因子认证用于帐户。

### 激活 PhoneFactor 认证
{: #cp_actphonefacauth}

添加 PhoneFactor 后，您必须通过客户门户网站使用 PhoneFactor 手动激活外部认证。由于 PhoneFactor 使用的是手动联系，因此务必确保与帐户关联的所有电话号码始终保持最新。如果未能保持更新联系人信息，那么可能会导致无法在 PhoneFactor 处于活动状态时访问客户门户网站和 VPN。成功添加 PhoneFactor 后，您将收到一封电子邮件，确认已添加 PhoneFactor。收到该电子邮件后，请使用以下步骤激活 PhoneFactor 认证。

1. 使用您的唯一凭证来访问客户门户网站。
2. 从导航栏中选择**帐户 > 用户**。
3. 单击用户名以访问该用户的关联用户概要文件。
4. 滚动至 **PhoneFactor 设置**部分。

  如果“PhoneFactor 设置”部分不可用，请首先验证您是否收到 PhoneFactor 供应电子邮件，指示已供应 PhoneFactor。如果 PhoneFactor 已供应，但该部分不可用，请创建支持凭单。如果 PhoneFactor 尚未供应，请等待电子邮件，然后重试。
  {: tip}

5. 从**状态**列表中，选择**活动**。
6. 编辑用于认证的**主电话号码**。
  1. 单击**编辑**链接。
  2. 在关联的字段中，输入**国家或地区代码**、**电话号码**和**分机**（如果适用）。
  3. 单击**认证并保存号码**以完成认证。

    添加用于认证的电话号码后，您必须在电话旁边等候。单击**认证**后，会呼叫该号码，并提示您完成号码认证步骤。如果不完成这些步骤，就无法对电话号码进行认证。
    {: tip}

  4. 要添加**辅助电话号码**，请重复上述步骤。
7. 从**方法**列表中，选择**联系方法**。
8. 从 **PIN 类型**列表中，选择一种 **PIN 类型**。
9. 如果选择**一次性** > **PIN 值**，请在 **PIN 值**字段中输入 PIN。
10. 单击**更新**以更新更改并激活 PhoneFactor 认证。

激活 PhoneFactor 后，客户门户网站或 VPN 需要通过 PhoneFactor 进行认证。使用用户凭证进行认证后，将显示一条消息，指示您正在尝试进行 PhoneFactor 认证。您或您要添加的用户必须在随 PhoneFactor 列出的电话旁边等候，以便完成认证。PhoneFactor 会尝试认证五次。五次认证尝试失败后，会将您锁定大约一小时。您或具有对帐户的管理访问权的用户可以随时更改 PhoneFactor 认证设置。您或帐户管理员可以随时停用 PhoneFactor。

 如果选择为客户门户网站和 VPN 登录设置 PhoneFactor，那么结果是有两个独立的 2FA 登录过程，一个针对客户门户网站，另一个针对 VPN。
 {: tip}

#### PhoneFactor 认证方法
{: #cp_phonefacauthmeths}

如果将 PhoneFactor 设置为认证类型，那么可以选择以下其中一个选项作为认证方法：

<dl>
<dt>电话呼叫和标准（无 PIN）</dt>
<dd>启用此选项后，当您登录到门户网站时，会收到对所启用的主号码的电话呼叫。接听电话时，会指示您按 # 键完成认证。</dd>
<dt>电话呼叫（使用 PIN）</dt>
<dd>选择此选项后，您将在客户门户网站中输入 PIN 值。PIN 必须是 4 到 8 位数字。当您尝试登录到门户网站时，会收到对门户网站中所列主号码的呼叫。接听电话时，会指示您输入 PIN 号并按 # 完成认证。</dd>
<dt>短信文本和一次性 PIN</dt>
<dd>选择此选项后，您将收到一条带 PIN 的短信，此 PIN 供您用于回复该消息。输入所提供的 PIN 后，即会完成认证过程，并登录到门户网站。</dd>
<dt>短信文本和一次性代码及 PIN 值</dt>
<dd>选择此选项后，您将创建 4 到 8 位数字的 PIN 值。然后，您会收到一条短信，您可使用提供的代码和您的 PIN 号（不含空格）进行回复。</dd>
<dt>PhoneFactor 应用程序和标准（无 PIN）</dt>
<dd>在设备上打开 PhoneFactor 应用程序 (Microsoft Authenticator)，然后单击<strong>认证</strong>。这将显示您已使用 PhoneFactor 成功认证且已登录到门户网站。</dd>
<dt>PhoneFactor 应用程序（使用 PIN）</dt>
<dd>使用此选项，您将在门户网站中设置 4 到 8 位数字的 PIN。然后，在设备上打开 PhoneFactor 应用程序 (Microsoft Authenticator)。接下来，输入在门户网站中所创建的 PIN，然后单击<strong>认证</strong>以登录到门户网站。</dd>
</dl>
