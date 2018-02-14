---

copyright:

  years: 1994, 2018

lastupdated: "2017-12-05"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 预订通知
{: #cp_bpnotifications}

有时，{{site.data.keyword.BluSoftlayer_notm}} 基础架构中会发生需要执行操作的事件；有些是意外事件，有些是保持 {{site.data.keyword.BluSoftlayer_notm}} 基础架构在其峰值条件下正常运行的计划维护活动。我们已尽可能使客户与这些事件相隔离，但有时还是需要使设备脱机。不管对客户有怎样的影响，始终需要做到信息透明、及时和翔实。
{:shortdesc}

您应该掌控自己的云体验，因此您需要及时了解有关维护活动的信息。要获取这些信息，您可以预订来自客户门户网站的通知。{{site.data.keyword.BluSoftlayer_notm}} 基础架构对以下类型的重要操作事件使用事件管理系统 (EMS) 通知过程：
* 计划外基础架构问题：在特定客户的特定条件下可能导致中断的问题
* 计划服务维护：使基础架构保持以最佳状态运行所需的维护
* 开具的支持凭单：向预订用户提醒在其帐户上开具的凭单

{{site.data.keyword.BluSoftlayer_notm}} 基础架构通知是专为云环境设计的，遵循以下重要原则：
* 通过客户门户网站自动执行
* 可扩展以访问不断增长的大型社区
* 有针对性地使 {{site.data.keyword.BluSoftlayer_notm}} 基础架构能够仅识别受该事件影响的客户和资源子集。

为了使通知系统完全生效，请预订该过程。如果你有需要通知的关键环境，还请确定 24 小时通知覆盖。

有关如何提供 {{site.data.keyword.BluSoftlayer_notm}} 基础架构通知的概述，请参阅 [Improving communications for customer-affecting planned events ![外部链接图标](../icons/launch-glyph.svg)](http://blog.softlayer.com/2014/improving-communications-customer-affecting-planned-events){:new_window}。

## 通知时间设置策略
{: #cp_bpgsnotiftimpol}

{{site.data.keyword.BluSoftlayer_notm}} 基础架构提前多长时间向用户通知暂挂事件不一定，具体取决于事件是计划外基础架构问题还是计划维护或安排的维护。一般情况下，{{site.data.keyword.BluSoftlayer_notm}} 基础架构策略是尽快补救问题，以消除或尽可能降低问题进一步发展而可能产生更大影响的风险。这意味着有时甚至执行计划维护也只提前很短的时间通知。

### 策略概述
{: #cp_bpgsnotifpolover}

您会收到以下类型的中断或问题的通知，如下面各部分中所述。

#### 计划外问题或中断
一旦了解了与基础架构范围、变通方法或解决方案估算相关的信息，{{site.data.keyword.BluSoftlayer_notm}} 基础架构会尽快向受影响的客户传达此信息。及时沟通可为您提供计划突发事件所需的信息，并确保 {{site.data.keyword.BluSoftlayer_notm}} 基础架构在解决此问题。

#### 安排的维护
{{site.data.keyword.BluSoftlayer_notm}} 基础架构会在安排的维护发生之前提供该事件的通知。有时候 {{site.data.keyword.BluSoftlayer_notm}} 基础架构维护属于紧急情况，这可能导致通知的提前时间更短。我们的目标始终是在提供合理的通知提前时间以允许您计划突发事件与升级或增强基础架构之间找到理想的平衡点，从而提高总体稳定性或增加所需功能。

#### 安全漏洞
{{site.data.keyword.BluSoftlayer_notm}} 基础架构会隔离受影响的区域，创建补丁来修复漏洞，并测试补丁以确保不会影响附带功能。这些工作往往会与可能提供受影响技术某些部分的其他供应商合作完成。通常，对于安全补丁会有公共通知禁发时间，此时间始终较短，以便保护公众，但这就需要缩短提前通知时间段。{{site.data.keyword.BluSoftlayer_notm}} 基础架构会赶在公众意识到问题之前，在受影响的整个基础架构上实施补丁，否则会增加风险。漏洞修复速度越快，风险消除的速度就越快，这意味着安全问题需要的通知时段较短。

安全漏洞更常见的其中一个目标是虚拟基础架构软件。{{site.data.keyword.BluSoftlayer_notm}} 基础架构使用常用的开放式源代码和合作伙伴技术来交付其虚拟服务器产品。要实施安全修订，运行虚拟基础架构软件的客户服务器可能必须脱机才能打补丁并重新引导环境，而这会导致中断。为了最大限度地降低对客户的影响，{{site.data.keyword.BluSoftlayer_notm}} 基础架构最近对虚拟基础架构的通知过程做了改进：改善了通信。对于每个 pod，客户接收通知时会使用特定开始时间和 90 分钟时段，这可缩短中断时间，并提供更准确的时间设置，以帮助您更好地做好准备。通知系统会隔离对每个帐户的维护工作，支持 {{site.data.keyword.BluSoftlayer_notm}} 基础架构在处理客户的特定主机时立即通知客户，这往往在 90 分钟时段之前很早的时候发生。

#### 多个受影响的 POD 或数据中心
除非情况极端紧急，必须实施修订以避免更大的间接影响，否则 {{site.data.keyword.BluSoftlayer_notm}} 基础架构会尽力提前更长时间发送通知。


## 向事件通知添加订户
{: #cp_bpaddsub2eventnotcp}

IBM 客户更多地依赖于 {{site.data.keyword.BluSoftlayer_notm}} 基础架构服务 (IaaS)，采用的方法是与 IBM 签订受管基础架构服务合同、针对在 {{site.data.keyword.BluSoftlayer_notm}} 基础架构上运行的云服务签订合同或直接与 {{site.data.keyword.BluSoftlayer_notm}} 基础架构服务签订合同。云服务涉及基础架构时，仅 SoftLayer 帐户用户有权接收通知，如上一部分中所述。在某些情况下，您在基础架构服务运营或支持中可能没有 IBM 客户或受管服务团队参与来访问您的 SoftLayer 帐户。为此，{{site.data.keyword.BluSoftlayer_notm}} 基础架构客户门户网站中添加了一项新功能，支持您指定订户（例如，IBM 人员）的列表，这些订户无需具有对您帐户的任何权限就可接收通知。

要指定订户列表，主用户可以登录到自己的客户门户网站帐户并使用以下步骤：
1. 从菜单中选择**帐户** > **管理** > **预订**。
2. 选择要向其添加订户的事件类型。
2. 从弹出窗口中，添加一个或多个电子邮件地址。电子邮件地址可以是 IBM 或非 IBM 的。
3. 单击**创建**。

作为额外订户添加的电子邮件地址将接收计划和计划外事件通知，以及开具的支持凭单。通知中包含技术详细信息，因此在添加订户时应考虑这些信息。由于通知的详细技术性质，目标订户应该是对通知将如何影响您的 {{site.data.keyword.BluSoftlayer_notm}} 基础架构环境知之甚详的人员。无法根据通知中的详细信息理解潜在客户影响的预订收件人会起到反效果，因此强烈建议不要使用这些收件人。
