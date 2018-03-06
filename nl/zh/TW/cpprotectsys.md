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


# 保護系統
{: #customerportal_protsys}

保護系統可確保系統流暢地執行，而且沒有不必要的岔斷。

## 使用專用網路
{: #cp_bpuseprivnet}

您可以使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構專用網路，在盡可能最安全的環境中管理裝置。盡可能使用 VPN 連線與裝置互動，並啟用網路跨越，讓系統透過專用網路進行通訊。若要存取專用網路，請從[使用者清單 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window} 中編輯使用者的 VPN 存取權。使用[虛擬專用網路 ![外部鏈結圖示](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} 指示，以連接至各種 VPN 選項的其中一個。

### 不要在公用網路上開啟 RDP、SSH 或控制埠
{: #cp_bpnordpsshcponpubnet}

公用網路對很多事情而言很棒，但某些特定層面如果透過開放的埠而保持提供於公用網路時，會讓系統出現漏洞。在公用網路上停用 RDP 或限制 SSH，即可保護您自己。如果必須在公用網路上使用這些服務，請考慮將 RDP 或 SSH 移至自訂埠號。

## 透過定期備份保護資料
{: #cp_bpsafedataregback}

{{site.data.keyword.BluSoftlayer_notm}} 基礎架構提供多個備份解決方案，確保您可以在磁碟機故障或使用者錯誤時擷取資料。備份解決方案目前包括 NAS、EVault Backup 及 R1Soft CDP，這些都會出現在各種儲存空間選項中。如需每一個備份解決方案的相關資訊，請參閱[儲存空間 ![外部鏈結圖示](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} 頁面。

### 不要假設您有備援；要確知您有
{: #cp_bpknowredundant}

{{site.data.keyword.BluSoftlayer_notm}} 基礎架構提供多個附加備援（包括雙重路徑、備用電源供應器及 RAID 配置）。請驗證您已佈建其中一個以上的特性，以確保您是在備援環境中工作，並且在失敗時受到保護。

### 確認先備份資訊然後再執行 OS 重新載入
{: #cp_bpnoperfOSwobackupconf}

重新載入作業系統會移除裝置硬碟中的所有資料。起始 OS 重新載入之前，請備份您的資訊，並驗證該備份成功，就不會遺失任何資訊。完成 OS 重新載入之後，即無法擷取遺失的資訊。

## 不要移除 Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用 ASM 來監視 RAID 陣列狀態。如果您刪除此軟體，則支援團隊無法監視裝置。如果從裝置中移除 ASM，則裝置上的 RAID 失敗警示無法使用，而且您無法透過自動通知系統接收到失敗通知。
