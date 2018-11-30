---

copyright:

  years: 1994, 2018

lastupdated: "2017-11-20"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# Rebooting your server
{: #customerportal_rebootserver}

Sometimes, events occur in {{site.data.keyword.BluSoftlayer_notm}} infrastructure that require you to restart your server.
{:shortdesc}

Use the following steps to restart your server:
1. From the customer portal, click the **Support** tab.
2. Click **reboot**.
3. Select the server to restart, and click **reboot**.
4. Select one of the following methods to restart the server:
  * Default (try the restart with IPMI and then with the power strip)
  * IPMI
  * Power strip
5. Click **reboot**.

This page also offers the ability to boot into the rescue kernel, which is very helpful if you're experiencing an issue in which the server can't boot to the OS because of a configuration issue. After booting to the rescue kernel, you can mount the drive, or drives, of your server and then fix the configuration issue. After the issue has been fixed, you can restart the server from the command line and the server will restart into the default kernel for your server. After you've issued the restart command, you'll see an estimated time of completion.
