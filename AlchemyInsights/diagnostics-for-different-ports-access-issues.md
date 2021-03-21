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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897486"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="980b4-102">診斷不同連接埠存取的問題</span><span class="sxs-lookup"><span data-stu-id="980b4-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="980b4-103">若要解決不同的連接埠存取問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="980b4-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="980b4-104">從入口網站停止/解除配置虛擬機器 (VM)，重新啟動虛擬機器，然後再次測試。</span><span class="sxs-lookup"><span data-stu-id="980b4-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="980b4-105">檢查虛擬機器的網路設定，以判斷您是否使用網路安全性群組 (NSG) 封鎖流量。</span><span class="sxs-lookup"><span data-stu-id="980b4-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="980b4-106">您也可以使用[網路觀察程式的 IP 流程驗證工具](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support)來檢查 NSG 是否有封鎖流量，使用者定義的路由 (UDR) 將您的流量重新路由回內部部署 (「預設路由」0.0.0.0/0) 或至網路應用裝置。</span><span class="sxs-lookup"><span data-stu-id="980b4-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="980b4-107">如果嘗試上述步驟後仍然發生問題，請提供您嘗試傳送郵件所在的虛擬機器名稱和 TCP 連接埠，以便進一步診斷。</span><span class="sxs-lookup"><span data-stu-id="980b4-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="980b4-108">**建議的文件**</span><span class="sxs-lookup"><span data-stu-id="980b4-108">**Recommended Documents**</span></span>

[<span data-ttu-id="980b4-109">透過連接埠 25 傳送外寄電子郵件的限制和建議</span><span class="sxs-lookup"><span data-stu-id="980b4-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)