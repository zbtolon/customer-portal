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

# 將伺服器重新開機
{: #customerportal_rebootserver}

有時，{{site.data.keyword.BluSoftlayer_notm}} 基礎架構中會發生需要您將伺服器重新開機的事件。
{:shortdesc}

請使用下列步驟，以將伺服器重新開機：
1. 從客戶入口網站中，按一下**支援**標籤。
2. 按一下**重新開機**。
3. 選取要重新開機的伺服器，然後按一下**重新開機**。
4. 選取下列其中一種方法，以將伺服器重新開機：
  * 預設（依序嘗試使用 IPMI 及配電板重新開機）
  * IPMI
  * 配電板
5. 按一下「重新開機」。

此頁面也可以開機到救援核心，這在您遇到伺服器因配置問題而無法開機到 OS 的問題時十分有用。開機到救援核心之後，您可以為伺服器裝載一個以上的磁碟機，然後修正配置問題。修正問題之後，即可從指令行將伺服器重新開機，而且伺服器會重新開機到您伺服器的預設核心。在您發出 reboot 指令之後，會看到估計完成時間。
