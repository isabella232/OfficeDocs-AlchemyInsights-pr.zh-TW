---
title: 讀取已刪除事件的審計記錄檔
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464434"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="7d795-102">讀取已刪除事件的審計記錄檔</span><span class="sxs-lookup"><span data-stu-id="7d795-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="7d795-103">以下說明如何執行此動作：</span><span class="sxs-lookup"><span data-stu-id="7d795-103">Here's how to do this:</span></span>

1. <span data-ttu-id="7d795-104">移至 [Office 365 的安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="7d795-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="7d795-105">選取 [**搜尋**  >  [**審核記錄搜尋**](https://go.microsoft.com/fwlink/?linkid=2103759)]。</span><span class="sxs-lookup"><span data-stu-id="7d795-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="7d795-106">如果您看到需要開啟此功能的通知，請繼續進行並開啟它。</span><span class="sxs-lookup"><span data-stu-id="7d795-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="7d795-107">如果未開啟此功能，搜尋結果將無法從先前的日期提取資料。</span><span class="sxs-lookup"><span data-stu-id="7d795-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="7d795-108">選取 [ **活動**]，然後尋找 [ **Exchange 信箱活動**]。</span><span class="sxs-lookup"><span data-stu-id="7d795-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="7d795-109">選取 [刪除的郵件] 資料夾 **中已刪除的郵件** ，並將 **郵件移至 [刪除** 的郵件] 資料夾選項。</span><span class="sxs-lookup"><span data-stu-id="7d795-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="7d795-110">當您完成時，按一下窗格外以最小化 [ **活動** ] 窗格。</span><span class="sxs-lookup"><span data-stu-id="7d795-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="7d795-111">指定日期範圍，然後在 [ **使用者** ] 方塊中，選取您要調查之使用者的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="7d795-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="7d795-112">您可以一次選取一個以上的使用者。</span><span class="sxs-lookup"><span data-stu-id="7d795-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="7d795-113">選取 [ **搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="7d795-113">Select **Search**.</span></span> <span data-ttu-id="7d795-114">活動會顯示在 [ **結果**] 底下。</span><span class="sxs-lookup"><span data-stu-id="7d795-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="7d795-115">若要查看詳細資料，請選取活動，然後選取 [ **詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="7d795-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="7d795-116">在 [ **AffectedItems** ] 欄位中會顯示刪除專案的其他資訊，例如專案的主旨行和位置。</span><span class="sxs-lookup"><span data-stu-id="7d795-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="7d795-117">您無法使用「審核記錄」功能還原已刪除的專案。</span><span class="sxs-lookup"><span data-stu-id="7d795-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="7d795-118">若要還原已刪除的專案，請參閱 [在 Outlook Web App 中復原刪除的郵件或電子郵件](https://go.microsoft.com/fwlink/?linkid=2103759)。</span><span class="sxs-lookup"><span data-stu-id="7d795-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="7d795-119">若要深入瞭解，請參閱 [搜尋 Office 365 audit log 以進行常見案例疑難排解](https://go.microsoft.com/fwlink/?linkid=2103944)。</span><span class="sxs-lookup"><span data-stu-id="7d795-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
