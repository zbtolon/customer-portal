---

copyright:

  years: 1994, 2018

lastupdated: "2018-11-28"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}


# 常见问题
{: #bicpfaq}

## 如何检索用于客户门户网站的凭证？
{: #bicp_retcreds}
{: faq}

如果您使用 IBM 标识进行认证，那么首次下订单时或将您添加为某个帐户的用户时，您将收到一封电子邮件，其中包含一个链接，供您开始使用 IBM 标识。如果丢失或忘记了您的用户名或密码，请转至 [IBM 标识概要文件 ![外部链接图标](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} 以重置或恢复密码。系统将提示您输入特定信息，其中可能包括创建安全问题的答案。

如果您不使用 IBM 标识进行认证，那么首次下订单时或将您添加为[客户门户网站 ![外部链接图标](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 帐户的用户时，您会收到一封电子邮件，其中包含您的用户名和初始密码，供您在客户门户网站中开始工作。首次登录后，请务必通过编辑用户概要文件来更改您的密码。

如果您登录后忘记了密码，请使用客户门户网站的登录屏幕上提供的**忘记密码**功能。系统将提示您输入特定信息，包括您在设置用户概要文件时指定的一组安全问题。

如果您忘记了用户名，请联系能够检索您的用户名的帐户管理员或主用户。如果您是帐户的管理员或主用户，请联系支持人员以获取更多帮助。

## 什么是 IBM 标识？
{: #bicp_whatisibmid}
{: faq}

新帐户需要 IBM 标识进行认证。现有帐户可继续使用 SoftLayer 用户名和密码进行认证，直到您运行迁移工具切换到 IBM 标识。SoftLayer 帐户有一个主用户，此用户有权在同一帐户中添加更多的用户。 

## 如何链接现有 SoftLayer 帐户？
{: #bicp_linkbmxacct}
{: faq}

如果您是 SoftLayer 帐户的主用户，请登录到客户门户网站并单击标题中的**链接帐户**。有关更多信息，请参阅[链接 IBM 标识用户帐户](/docs/account/softlayerlink.html)。

## 我必须是现有 {{site.data.keyword.Bluemix_notm}} 用户才能链接帐户吗？
{: #bicp_bmxusertolink}
{: faq}

不，您可以创建新的 {{site.data.keyword.Bluemix_notm}} 帐户，也可以链接现有的 {{site.data.keyword.Bluemix_notm}} 轻量或现买现付帐户。

## 双因子认证如何工作？
{: #bicp_2fa}
{: faq}

对帐户级别的双因子认证 (2FA) 配置没有影响。2FA 不是按 IBM 标识的，它仍是按帐户的。当一个 IBM 标识与多个帐户相关联，而您在各帐户之间进行切换时，每次切换到要求 2FA 的不同帐户时都必须确认身份。即使旧帐户和新帐户都配置了相同的 2FA 机制，也是如此。

有关使用 2FA 的 IBM 标识的更多信息，请参阅[链接的帐户中的多因子认证用法](/docs/account/softlayerlink.html#2fa)。

## 谁可以链接帐户？
{: #bicp_wholinkaccts}
{: faq}

只有 {{site.data.keyword.BluSoftlayer_notm}} 基础架构主用户可以链接 SoftLayer 和 {{site.data.keyword.Bluemix_notm}} 帐户。主用户的电子邮件还必须关联到所链接的 {{site.data.keyword.Bluemix_notm}} 帐户的主要所有者。

## 我将使用什么来登录每个控制台？
{: #bicp_logineachport}
{: faq}

您的帐户记帐已链接，所以您可以轻松在 SoftLayer 和 {{site.data.keyword.Bluemix_notm}} 帐户之间移动，但您的帐户身份保持独立。

* 如果您的帐户不使用 IBM 标识进行认证，请继续将 SoftLayer 标识用于 SoftLayer 产品和服务，并将 IBM 标识用于 {{site.data.keyword.Bluemix_notm}} 产品和服务。

* 如果您的帐户使用 IBM 标识进行认证，那么您可使用 IBM 标识来访问 SoftLayer 和 {{site.data.keyword.Bluemix_notm}} 帐户。

## 为何在尝试使用我的 SoftLayer 用户名登录时收到错误？
{: #bicp_SLloginerror}
{: faq}

切换到 IBM 标识后，如果使用您的 {{site.data.keyword.BluSoftlayer_notm}} 基础架构用户名登录到客户门户网站，将显示“提供的登录凭证无效”错误。在切换到 IBM 标识后，您不能再使用 {{site.data.keyword.BluSoftlayer_notm}} 基础架构用户名来登录到客户门户网站。您必须在“帐户登录”对话框中单击**使用 IBM 标识登录**。

## 为何在尝试使用我的 IBM 标识登录时收到错误？
{: #bicp_IBMidloginerror}
{: faq}

在使用 IBM 标识登录时，将显示“无法识别此 IBM 标识或电子邮件”错误。确保输入标准电子邮件地址。另请确保您使用的不是 {{site.data.keyword.BluSoftlayer_notm}} 基础架构用户名。

## {{site.data.keyword.BluSoftlayer_notm}} 基础架构团队成员能否访问链接的帐户？
{: #bicp_linkgiveteamaccess}
{: faq}

您必须邀请他们加入 {{site.data.keyword.Bluemix_notm}}。在 {{site.data.keyword.Bluemix_notm}} 控制台中，单击**管理** > **帐户** > **用户**。在选择资源组后，您可以添加 {{site.data.keyword.BluSoftlayer_notm}} 基础架构团队成员。您可能必须登录到客户门户网站后，才能发送邀请。{{site.data.keyword.Bluemix_notm}} 会获取 {{site.data.keyword.BluSoftlayer_notm}} 基础架构用户的列表，然后您可以选择要邀请加入 {{site.data.keyword.Bluemix_notm}} 帐户的用户。

## 用于完成切换到 IBM 标识的过程的电子邮件在哪里？
{: #bicp_ibmidswitchemail}
{: faq}

如果您遵循向导切换到 IBM 标识，但没有收到相应电子邮件，这是因为可能需要几分钟到几小时才会将包含注册代码的电子邮件发送给您。您可以返回到客户门户网站中的**编辑用户概要文件**页面，然后单击**重新发送电子邮件**以重试。

## 我是否拥有对我的帐户的完全 root 用户访问权？
{: #bicp_fullrootaccaccess}
{: faq}

主用户和具有管理员许可权的用户对客户门户网站和 API 上的帐户具有完全 root 用户访问权。没有管理员许可权的用户的可访问性由具有管理员角色的用户进行控制。在客户门户网站中，管理员可以通过[编辑用户概要文件](/docs/customer-portal/cpmanuserprof.html#cp_edituserprofile)来更新这些许可权。如果您没有管理员许可权，那么可以在客户门户网站中通过单击顶部面板上的用户名来编辑用户概要文件。

## 可以链接 {{site.data.keyword.Bluemix_notm}} 预订帐户吗？
{: #bicp_linkbmxsubacct}
{: faq}

{{site.data.keyword.Bluemix_notm}} 中的所有链接帐户都必须是轻量或现买现付帐户。 

## 如何取消链接帐户？
{: #bicp_unlinkacct}
{: faq}

帐户链接之后即无法对其取消链接。


## 什么是公司概要文件？我在哪里可以找到该文件？
{: #bicp_whatfindcompprof}
{: faq}

公司概要文件是在创建帐户时提交的信息，包括公司的主要联系人以及公司名称、地址和电话号码。出于各种原因会使用这些信息，因此这些信息应始终保持最新。要查看您帐户的公司概要文件或要请求更改，请参阅[更新公司概要文件](/docs/customer-portal/cpmanacctcompprofcont.html#cp_updcompprof)。

## 在哪里可以找到设备和软件密码？
{: #bicp_devswpw}
{: faq}

设备和软件密码存储在客户门户网站中的两个位置。要检索设备凭证（包括 {{site.data.keyword.baremetal_short}} 和 {{site.data.keyword.virtualmachinesshort}} 的 root 用户或管理员用户的用户名和密码），请参阅[在快照视图中与设备交互](/docs/vsi/vsi_interact_device_snapshot_view.html)。要使用客户门户网站快速查看和检索手动跟踪的软件凭证，请参阅[管理设备访问权](/docs/vsi/vsi_device_access.html)。

## 如何使 Web 数据保持同步？
{: #bicp_webdatasync}
{: faq}

虽然由您负责使真实服务器之间的数据保持一致，但 {{site.data.keyword.BluSoftlayer_full}} 提供了一个专用网络，您可以使用该网络进行同步，而不会产生使用费用。

## 什么是事件管理系统？
{: #bicp_whatisems}
{: faq}

事件管理系统是一个工具集，用于优化 {{site.data.keyword.BluSoftlayer_full}} 与用户共享计划外基础架构问题和即将到来的计划维护事件相关信息的方式。该系统使用针对这些事件的基于预订的目标电子邮件警报来共享所发生事件的类型。此外，该系统还为预订用户提供有关事件总体影响和进行中计划外事件 (UIP) 的当前状态的详细信息。

## 可以取消设备吗？
{: #bicp_candev}
{: faq}

您可以通过客户门户网站随时取消设备。有关完成取消请求的更多信息，请参阅[取消设备](/docs/vsi/vsi_managing.html)。
