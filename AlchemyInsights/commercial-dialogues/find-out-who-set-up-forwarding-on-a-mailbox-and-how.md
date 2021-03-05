---
title: 瞭解誰會在信箱上設定轉發，以及如何
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464438"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="f6047-102">瞭解誰會在信箱上設定轉發，以及如何</span><span class="sxs-lookup"><span data-stu-id="f6047-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="f6047-103">如果在信箱上設定外部轉寄，該活動會在 Set-Mailbox Cmdlet 中進行審核。</span><span class="sxs-lookup"><span data-stu-id="f6047-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="f6047-104">以下說明如何在審計記錄檔中尋找活動：</span><span class="sxs-lookup"><span data-stu-id="f6047-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="f6047-105">移至 [Office 365 的安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="f6047-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f6047-106">選取 [**搜尋** >  **審核記錄搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="f6047-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f6047-107">如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。</span><span class="sxs-lookup"><span data-stu-id="f6047-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f6047-108">若未開啟此功能，搜尋結果將無法從先前的日期提取資料。</span><span class="sxs-lookup"><span data-stu-id="f6047-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f6047-109">請確定 [ **活動** ] 欄位已設定為顯示預設)  (**所有活動的結果** 。</span><span class="sxs-lookup"><span data-stu-id="f6047-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="f6047-110">指定日期範圍。</span><span class="sxs-lookup"><span data-stu-id="f6047-110">Specify the date range.</span></span> <span data-ttu-id="f6047-111">您不需要指定使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="f6047-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="f6047-112">選取 [ **搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="f6047-112">Select **Search**.</span></span> <span data-ttu-id="f6047-113">活動會顯示在 [ **結果**] 底下。</span><span class="sxs-lookup"><span data-stu-id="f6047-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="f6047-114">選取 [**篩選結果**]，然後在 [**活動** 篩選] 欄位中輸入 **集信箱**。</span><span class="sxs-lookup"><span data-stu-id="f6047-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="f6047-115">這會傳回所有的 **Set-Mailbox** 活動。</span><span class="sxs-lookup"><span data-stu-id="f6047-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="f6047-116">若要查看詳細資料，請選取活動，然後選取 [ **詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="f6047-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="f6047-117">在 [ **參數** ] 底下您可以看到信箱上設定的轉寄電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="f6047-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="f6047-118">**UserID** 代表在信箱上設定外部轉送的使用者。</span><span class="sxs-lookup"><span data-stu-id="f6047-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="f6047-119">若要深入瞭解，請參閱 [搜尋 Office 365 audit log 以進行常見案例疑難排解](https://go.microsoft.com/fwlink/?linkid=2103944)。</span><span class="sxs-lookup"><span data-stu-id="f6047-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>