---
title: Microsoft 365 中的審計
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464445"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="884b0-102">Microsoft 365 中的審計</span><span class="sxs-lookup"><span data-stu-id="884b0-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="884b0-103">以下是您在 Microsoft 365 中的審計應注意的一些事項：</span><span class="sxs-lookup"><span data-stu-id="884b0-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="884b0-104">預設會審核 Exchange 系統管理員活動。</span><span class="sxs-lookup"><span data-stu-id="884b0-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="884b0-105">我們正在為所有使用者預設開啟信箱審核的處理常式。</span><span class="sxs-lookup"><span data-stu-id="884b0-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="884b0-106">若要進一步閱讀此資訊，請按一下 [這裡](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)。</span><span class="sxs-lookup"><span data-stu-id="884b0-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="884b0-107">在此之前，如果您想要將其手動啟用一人或整個組織的指示，請選擇下面的 [開啟信箱審核] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="884b0-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="884b0-108">Microsoft 365 群組信箱和公用資料夾信箱不支援審計記錄。</span><span class="sxs-lookup"><span data-stu-id="884b0-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="884b0-109">若為 SharePoint/OneDrive，啟用審核時，不需要進行其他設定。</span><span class="sxs-lookup"><span data-stu-id="884b0-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="884b0-110">若要瞭解所審核的活動，請參閱：</span><span class="sxs-lookup"><span data-stu-id="884b0-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="884b0-111">檔案活動</span><span class="sxs-lookup"><span data-stu-id="884b0-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="884b0-112">資料夾活動</span><span class="sxs-lookup"><span data-stu-id="884b0-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="884b0-113">[共用和存取活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)。</span><span class="sxs-lookup"><span data-stu-id="884b0-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="884b0-114">如需服務的所有已審核活動的清單，請參閱已 [審核的活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)。</span><span class="sxs-lookup"><span data-stu-id="884b0-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
