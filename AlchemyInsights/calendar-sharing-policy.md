---
title: 618行事曆共用原則
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684221"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="2f8a8-102">共用行事歷時的原則錯誤</span><span class="sxs-lookup"><span data-stu-id="2f8a8-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="2f8a8-103">請視情況而定，請執行下列其中一項動作：</span><span class="sxs-lookup"><span data-stu-id="2f8a8-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="2f8a8-104">使用遠端 PowerShell 連接至 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="2f8a8-105">如需詳細資訊，請參閱 [Connect To Exchange Online Using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="2f8a8-106">在內部部署伺服器上，開啟 Exchange 管理命令介面。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="2f8a8-107">決定指派給使用者的共用原則。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="2f8a8-108">若要這麼做，請執行下列命令，並記下傳回的原則：</span><span class="sxs-lookup"><span data-stu-id="2f8a8-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="2f8a8-109">更新使用者的共用原則。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="2f8a8-110">如果要執行這項操作，請依照下列步驟執行：</span><span class="sxs-lookup"><span data-stu-id="2f8a8-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="2f8a8-111">開啟 [Exchange 系統管理中心]。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="2f8a8-112">按一下 [ **組織**]，然後按兩下 [ **個人共用**] 下指派給使用者的原則。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="2f8a8-113">這是在步驟2中傳回的原則。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="2f8a8-114">在 [共用規則] 頁面上，在 [ **指定您要共用的資訊**] 下，選取您想要允許的行事曆共用層級。按一下 [ **儲存**]。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="2f8a8-115">如需詳細資訊，請參閱：「 [原則不允許將此層級的許可權授與一個或多個收件者 (s) 」當使用者嘗試共用行事歷時，發生錯誤](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)。</span><span class="sxs-lookup"><span data-stu-id="2f8a8-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
