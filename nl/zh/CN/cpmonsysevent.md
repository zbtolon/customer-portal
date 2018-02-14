---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-01"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# 监视 {{site.data.keyword.Bluemix_notm}} 基础架构系统事件
{: #customerportal_monevent}

您可以监视系统事件以保持系统平稳运行。有关在 {{site.data.keyword.BluSoftlayer_full}} 基础架构中设置和管理虚拟服务器的信息，请参阅[虚拟服务器入门](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers)。
{:shortdesc}

## 查看帐户的审计日志
{: #cp_viewacctauditlog}

每个客户门户网站帐户均随附审计日志，用于跟踪客户门户网站内每个用户的交互。跟踪的交互包括登录尝试（成功和失败）、端口速度更新、开机或关机和重新引导以及由 {{site.data.keyword.BluSoftlayer_notm}} 基础架构支持人员所进行的交互。使用以下步骤查看用户帐户的审计日志。

1. 使用您的唯一凭证访问[客户门户网站 ![外部链接图标](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 从导航栏中选择**帐户** > **管理** > **审计日志**以访问审计日志。

审计日志初始会显示帐户上的用户所做的最后 25 个交互。您可以随时查看多达 200 个交互。更新**显示**下拉列表中显示的结果数。如果更改了设置，那么交互的**操作**列将包含链接。单击任一链接可查看受此操作影响的设置以及有关更改的详细信息。单击任何交互的设备名或用户名可分别使您重定向到“设备详细信息”屏幕或“用户概要文件”屏幕。

## 查看用户的访问日志
{: #cp_viewuserlogs}

访问日志显示由特定客户门户网站用户进行的每次访问尝试的数据。该日志显示每次访问尝试的日期和时间戳记以及 IP 地址。使用以下步骤查看用户的访问日志。

1. 使用您的唯一凭证访问[客户门户网站 ![外部链接图标](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}。
2. 从菜单栏中选择**帐户** > **用户**以访问“用户”窗口。
3. 从**操作**下拉列表中，选择**查看审计日志**以查看用户的访问日志。

每个用户的访问日志都会按日期显示该用户进行的访问尝试，以及用于进行访问尝试的 IP 地址。访问日志中的信息是只读的，因此无法随时对其内容进行编辑。您可以通过重复上述步骤，随时重新查看访问日志。要退出日志并返回到“用户”屏幕，请单击屏幕顶部的**查看所有用户**链接。
