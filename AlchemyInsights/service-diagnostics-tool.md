---
title: 用於 Windows 虛擬桌面的服務診斷工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590278"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="1deb2-102">用於 Windows 虛擬桌面的服務診斷工具</span><span class="sxs-lookup"><span data-stu-id="1deb2-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="1deb2-103">Windows 虛擬桌面 (WVD) 提供了可讓系統管理員透過單一介面識別錯誤的診斷工具。</span><span class="sxs-lookup"><span data-stu-id="1deb2-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="1deb2-104">當被指派 WVD 角色的人員使用 WVD 時，此工具會記錄診斷相關資訊。</span><span class="sxs-lookup"><span data-stu-id="1deb2-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="1deb2-105">每個記錄都包含有關活動中涉及的 WVD 角色之資訊、工作階段期間出現的錯誤訊息以及有關租用戶和使用者的資訊。</span><span class="sxs-lookup"><span data-stu-id="1deb2-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="1deb2-106">Azure 記錄分析可設定為透過以下步驟擷取診斷工具建立的活動記錄：</span><span class="sxs-lookup"><span data-stu-id="1deb2-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="1deb2-107">使用 [Azure 入口網站](https://go.microsoft.com/fwlink/?linkid=2129500)或 [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501) 建立記錄分析工作區。</span><span class="sxs-lookup"><span data-stu-id="1deb2-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="1deb2-108">[將 Windows 電腦連線至 Azure 監視器](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="1deb2-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="1deb2-109">取得工作區識別碼和工作區主索引鍵。</span><span class="sxs-lookup"><span data-stu-id="1deb2-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="1deb2-110">設定精靈需要此資訊來正確設定代理程式並確定它可以與 Azure 監視器通訊。</span><span class="sxs-lookup"><span data-stu-id="1deb2-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="1deb2-111">[將診斷資料推送至工作區](https://go.microsoft.com/fwlink/?linkid=2128284)。</span><span class="sxs-lookup"><span data-stu-id="1deb2-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="1deb2-112">您可以將 WVD 租用戶中的診斷資料推送至工作區的記錄分析。</span><span class="sxs-lookup"><span data-stu-id="1deb2-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="1deb2-113">[識別和診斷](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)與 WVD 相關的內部或外部問題。</span><span class="sxs-lookup"><span data-stu-id="1deb2-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="1deb2-114">若要深入了解為 WVD 設定服務診斷工具的資訊，請參閱使用記錄分析進行診斷功能。</span><span class="sxs-lookup"><span data-stu-id="1deb2-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>