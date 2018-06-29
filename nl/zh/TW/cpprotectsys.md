---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-30"

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

您可以使用 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構專用網路，在盡可能最安全的環境中管理裝置。盡可能使用 VPN 連線與裝置互動，並啟用網路跨越，讓系統透過專用網路進行通訊。若要存取專用網路，請從[使用者清單 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/account/user/list){:new_window} 中編輯使用者的 VPN 存取權。使用[虛擬專用網路 ![外部鏈結圖示](../icons/launch-glyph.svg)](http://www.softlayer.com/vpn-access){:new_window} 清單，以連接至各種 VPN 選項的其中一個。

如需使用 VPN 連線的相關資訊，請參閱[關於 VPN](/docs/infrastructure/iaas-vpn/about-vpn.html)。

### 不要在公用網路上開放 RDP、SSH 或控制埠
{: #cp_bpnordpsshcponpubnet}

公用網路對很多事情而言很棒，但在某些層面，如果在公用網路上提供開放埠，會讓系統出現漏洞。在公用網路上停用 RDP 或限制 SSH，即可保護您自己。如果必須在公用網路上使用這些服務，請考慮將 RDP 或 SSH 移至自訂埠號。

## 透過定期備份保護資料
{: #cp_bpsafedataregback}

排定備份以確保您的資料安全地儲存於裝置之外，且能在資料遺失時重新載入。

{{site.data.keyword.BluSoftlayer_notm}} 基礎架構提供多個備份解決方案，確保您可以在磁碟機故障或使用者犯錯時擷取資料。備份解決方案目前包括 NAS、EVault 備份及 R1Soft CDP，這些會以各種儲存空間選項提供。例如，您可以選擇下列其中一項備份服務，將您的資料儲存在安全的位置：
  * EVault 備份是一種以代理程式為基礎的自動化備份系統，且是用於管理裝置的熱門「設定後即忘記」解決方案。它透過其他外掛程式而與包括 Exchange 和 SQL 的 Microsoft 軟體相容。EVault 使用者可以透過 EVault 的 WebCC Web 型應用程式與此服務進行互動。
  * R1Soft Continuous Data Protection (CDP) 可以安裝在您的伺服器或自我管理的虛擬機器上。如果您要尋找的是以單一介面來管理所有的備份，則可以使用此產品。您可透過專有管理系統與 R1Soft CDP 互動，而此管理系統容許代理程式安裝在虛擬機器上，並且會提供資料庫外掛程式來提供更多功能。

 如需每一個備份解決方案的相關資訊，請參閱[儲存空間 ![外部鏈結圖示](../icons/launch-glyph.svg)](http://www.softlayer.com/services/storagelayer/){:new_window} 頁面，如需備份資料的相關資訊，請參閱[開始使用備份服務](/docs/infrastructure/Backup/index.html)。

### 不要假設您有備援；要確知您有
{: #cp_bpknowredundant}

{{site.data.keyword.BluSoftlayer_notm}} 基礎架構提供多個附加備援，包括雙重路徑、備用電源供應器及 RAID 配置。請驗證您已佈建其中一個以上的特性，以確保您是在備援環境中工作，並且在發生失敗的情況下受到保護。

### 確認已備份資訊然後再重新載入 OS
{: #cp_bpnoperfOSwobackupconf}

重新載入作業系統會移除裝置硬碟中的所有資料。起始 OS 重新載入之前，請備份您的資訊，並驗證該備份成功，就不會遺失任何資訊。完成 OS 重新載入之後，即無法擷取遺失的資訊。

## 不要移除 Adaptec Storage Manager (ASM)
{: #cp_bpsupdontremovasm}

 {{site.data.keyword.BluSoftlayer_notm}} 基礎架構使用 ASM 來監視 RAID 陣列狀態。如果您刪除此軟體，則支援團隊無法監視裝置。如果從裝置中移除 ASM，則裝置上的 RAID 失敗警示無法使用，而且您無法透過自動通知系統接收到失敗通知。
