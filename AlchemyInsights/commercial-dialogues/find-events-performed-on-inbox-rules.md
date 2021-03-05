---
title: 尋找對收件匣規則執行的事件
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464502"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="8f6cf-102">尋找對收件匣規則執行的事件</span><span class="sxs-lookup"><span data-stu-id="8f6cf-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="8f6cf-103">建立、變更或刪除收件匣規則時，事件會記錄在審計記錄檔中。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="8f6cf-104">以下說明如何進行檢查：</span><span class="sxs-lookup"><span data-stu-id="8f6cf-104">Here's how to review them:</span></span>

1. <span data-ttu-id="8f6cf-105">移至 [Office 365 的安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="8f6cf-106">選取 [搜尋] > [審計記錄搜尋]。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8f6cf-107">如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="8f6cf-108">若未開啟此功能，搜尋結果將無法從先前的日期提取資料。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="8f6cf-109">選取 [活動] 欄位，並尋找 Exchange 信箱活動，然後選取 [New-InboxRule 從 Outlook Web App 建立收件匣規則]。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="8f6cf-110">當您完成時，按一下窗格外以最小化 [活動] 窗格。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="8f6cf-111">指定日期範圍，然後在 [使用者] 欄位中，選取您要調查之使用者的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="8f6cf-112">您可以一次選取一個以上的使用者。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="8f6cf-113">選取 [搜尋]。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-113">Select Search.</span></span> <span data-ttu-id="8f6cf-114">活動會顯示在 [結果] 底下。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="8f6cf-115">若要查看詳細資料，請選取活動，然後選取 [詳細資訊]。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="8f6cf-116">在 [參數] 區段中，您可以看到規則的名稱、條件集，以及規則將採取的動作。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="8f6cf-117">若要深入瞭解，請參閱搜尋 Office 365 audit log 以進行常見案例疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8f6cf-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>