---
title: 618行事曆共用原則
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372990"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="891de-102">共用行事歷時的原則錯誤</span><span class="sxs-lookup"><span data-stu-id="891de-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="891de-103">請視情況而定，請執行下列其中一項動作：</span><span class="sxs-lookup"><span data-stu-id="891de-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="891de-104">使用遠端 PowerShell 連接至 Exchange Online。</span><span class="sxs-lookup"><span data-stu-id="891de-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="891de-105">如需詳細資訊，請參閱[Connect To Exchange Online Using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="891de-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="891de-106">在內部部署伺服器上，開啟 Exchange 管理命令介面。</span><span class="sxs-lookup"><span data-stu-id="891de-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="891de-107">決定指派給使用者的共用原則。</span><span class="sxs-lookup"><span data-stu-id="891de-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="891de-108">若要這麼做，請執行下列命令，並記下傳回的原則：</span><span class="sxs-lookup"><span data-stu-id="891de-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="891de-109">更新使用者的共用原則。</span><span class="sxs-lookup"><span data-stu-id="891de-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="891de-110">若要這樣做，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="891de-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="891de-111">開啟 [Exchange 系統管理中心]。</span><span class="sxs-lookup"><span data-stu-id="891de-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="891de-112">按一下 [**組織**]，然後按兩下 [**個人共用**] 下指派給使用者的原則。</span><span class="sxs-lookup"><span data-stu-id="891de-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="891de-113">這是在步驟2中傳回的原則。</span><span class="sxs-lookup"><span data-stu-id="891de-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="891de-114">在 [共用規則] 頁面上，在 [**指定您要共用的資訊**] 下，選取您想要允許的行事曆共用層級。按一下 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="891de-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="891de-115">如需詳細資訊，請參閱：「[原則不允許將此層級的許可權授與一或多個收件者（s）」在使用者嘗試共用行事歷時發生錯誤](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)。</span><span class="sxs-lookup"><span data-stu-id="891de-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
