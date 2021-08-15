---
title: 診斷不同連接埠存取的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030893"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>診斷不同連接埠存取的問題

若要解決不同的連接埠存取問題，請執行下列步驟：

1. 從入口網站停止/解除配置虛擬機器 (VM)，重新啟動虛擬機器，然後再次測試。 
2. 檢查虛擬機器的網路設定，以判斷您是否使用網路安全性群組 (NSG) 封鎖流量。 您也可以使用[網路觀察程式的 IP 流程驗證工具](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)來檢查 NSG 是否有封鎖流量，使用者定義的路由 (UDR) 將您的流量重新路由回內部部署 (「預設路由」0.0.0.0/0) 或至網路應用裝置。
如果嘗試上述步驟後仍然發生問題，請提供您嘗試傳送郵件所在的虛擬機器名稱和 TCP 連接埠，以便進一步診斷。

**建議的文件**

[透過連接埠 25 傳送外寄電子郵件的限制和建議](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)