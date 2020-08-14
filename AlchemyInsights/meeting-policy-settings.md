---
title: 會議原則設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042835"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6c397-102">在 Microsoft 小組中管理會議原則</span><span class="sxs-lookup"><span data-stu-id="6c397-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6c397-103">**附注：原則變更可能需要24小時才能讓使用者生效。**</span><span class="sxs-lookup"><span data-stu-id="6c397-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="6c397-104">您可能無法立即對新建立的原則進行變更。等候4小時，然後嘗試再次修改新建立的原則。</span><span class="sxs-lookup"><span data-stu-id="6c397-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="6c397-105">會議原則是用來控制會議參與者對於由組織中的使用者排程的會議參與者可用的功能。</span><span class="sxs-lookup"><span data-stu-id="6c397-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6c397-106">會議原則的某些功能可能無法在團隊系統管理中心中實施，但 (這些功能會在檔) 中標示為「即將推出」。</span><span class="sxs-lookup"><span data-stu-id="6c397-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6c397-107">在此情況下，或是如果您收到錯誤（如「我們無法立即更新原則，但稍後再試一次」）在 Microsoft 團隊系統管理中心，我們建議您使用 PowerShell 建立或修改小組會議原則。</span><span class="sxs-lookup"><span data-stu-id="6c397-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6c397-108">如需會議原則的詳細資訊，請參閱下列資源：</span><span class="sxs-lookup"><span data-stu-id="6c397-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6c397-109">若要瞭解如何建立原則、進行變更，以及將使用者指派給原則，請參閱 [管理小組中的會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="6c397-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6c397-110">若要使用 PowerShell Cmdlet 進行原則變更，請參閱 [團隊 PowerShell 綜述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。</span><span class="sxs-lookup"><span data-stu-id="6c397-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6c397-111">您需要針對團隊會議原則使用 [商務用 Skype PowerShell 模組](https://www.microsoft.com/download/details.aspx?id=39366) 。</span><span class="sxs-lookup"><span data-stu-id="6c397-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6c397-112">如需詳細資訊，請參閱 [\*-CsTeamsMeetingPolicy Cmdlet 檔](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 。</span><span class="sxs-lookup"><span data-stu-id="6c397-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

