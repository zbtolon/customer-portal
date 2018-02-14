---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-04"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 监视环境和系统事件
{: #customerportal_cpmonenvsysevent}

监视环境意味着您可以随时检查设备，并且在某个设备发生故障时自动收到通知。您还可以监视系统事件以保持系统平稳运行。  
{: shortdesc}

## 监视环境
{: #cpmonenv}

至少使用基本的 ping 监视，但您也可以使用最适合您的业务需求的方式来定制监视选项。

### 随时了解网络维护和计划外事件
{: #cp_stayinfomaintevent}

有时，执行安排的网络维护和紧急网络维护是不可避免的。{{site.data.keyword.BluSoftlayer_full}} 基础架构会维护许多通道（例如 [Twitter 帐户 ![外部链接图标](../icons/launch-glyph.svg)](https://twitter.com/softlayernotify){:new_window}），以便及时向您通知所有安排的维护事件和紧急维护事件。此外，可以通过事件管理系统[预订电子邮件通知 ](/docs/customer-portal/cpsub2not.html){:new_window}。此免费服务会自动向预订用户发送有关可能影响服务的计划外事件的电子邮件。

### 使用 {{site.data.keyword.BluSoftlayer_notm}} Infrastructure Mobile
{: #cp_bmxinframobile}

使用 [{{site.data.keyword.BluSoftlayer_notm}} Infrastructure Mobile ![外部链接图标](../icons/launch-glyph.svg)](https://knowledgelayer.softlayer.com/topic/mobile-devices){:new_window} 来使用 iOS 或 Android 移动设备持续管理 {{site.data.keyword.BluSoftlayer_notm}} 基础架构设备。{{site.data.keyword.BluSoftlayer_notm}} Infrastructure Mobile 中的功能包括开具凭单支持、基本设备控制和带宽监视。

## 监视系统事件
{: #customerportal_monevent}

可以通过查看审计日志和访问日志来监视系统事件。

### 查看帐户的审计日志
{: #cp_viewacctauditlog}

每个客户门户网站帐户均随附审计日志，用于跟踪客户门户网站内每个用户的交互。跟踪的交互包括登录尝试（成功和失败）、端口速度更新、开机或关机和重新引导以及由 {{site.data.keyword.BluSoftlayer_notm}} 基础架构支持人员所进行的交互。使用以下步骤查看用户帐户的审计日志。

1. 使用您的唯一凭证访问[客户门户网站 ![外部链接图标](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 从导航栏中选择**帐户** > **管理** > **审计日志**以访问审计日志。

审计日志初始会显示帐户上的用户所做的最后 25 个交互。您可以随时查看多达 200 个交互。更新**显示**下拉列表中显示的结果数。如果更改了设置，那么交互的**操作**列将包含链接。单击任一链接可查看受此操作影响的设置以及有关更改的详细信息。单击任何交互的设备名或用户名可分别使您重定向到“设备详细信息”屏幕或“用户概要文件”屏幕。

### 查看用户的访问日志
{: #cp_viewuserlogs}

访问日志显示由特定客户门户网站用户进行的每次访问尝试的数据。该日志显示每次访问尝试的日期和时间戳记以及 IP 地址。使用以下步骤查看用户的访问日志。

1. 使用您的唯一凭证访问[客户门户网站 ![外部链接图标](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 从菜单栏中选择**帐户** > **用户**以访问“用户”窗口。
3. 从**操作**下拉列表中，选择**查看审计日志**以查看用户的访问日志。

每个用户的访问日志都会按日期显示该用户进行的访问尝试，以及用于进行访问尝试的 IP 地址。访问日志中的信息是只读的，因此无法随时对其内容进行编辑。您可以通过重复上述步骤，随时重新查看访问日志。要退出日志并返回到“用户”屏幕，请单击屏幕顶部的**查看所有用户**链接。
