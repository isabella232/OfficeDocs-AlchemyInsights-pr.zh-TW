---
title: 在審計記錄檔中尋找 IP 位址
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464505"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="f2322-102">在審計記錄檔中尋找 IP 位址</span><span class="sxs-lookup"><span data-stu-id="f2322-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="f2322-103">對應至使用者或系統管理員所執行之活動的 IP 位址會顯示在審計記錄檔中。</span><span class="sxs-lookup"><span data-stu-id="f2322-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="f2322-104">也會記錄用戶端資訊。</span><span class="sxs-lookup"><span data-stu-id="f2322-104">The client information is also logged.</span></span> <span data-ttu-id="f2322-105">以下說明如何識別 IP 位址：</span><span class="sxs-lookup"><span data-stu-id="f2322-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="f2322-106">移至 [Office 365 的安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。</span><span class="sxs-lookup"><span data-stu-id="f2322-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f2322-107">選取 [**搜尋**  >  **[審核記錄搜尋](https://go.microsoft.com/fwlink/?linkid=2103759)**]。</span><span class="sxs-lookup"><span data-stu-id="f2322-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f2322-108">如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。</span><span class="sxs-lookup"><span data-stu-id="f2322-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f2322-109">如果未啟用此功能，搜尋結果將無法從先前的日期提取資料。</span><span class="sxs-lookup"><span data-stu-id="f2322-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f2322-110">如果您對特定活動感興趣，請從 [活動] 清單中進行選取，然後按一下 [ **活動** ] 清單。否則，預設會為選取的使用者傳回所有活動。</span><span class="sxs-lookup"><span data-stu-id="f2322-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="f2322-111">請注意，[ **活動** ] 功能表中可能無法選取某些活動;不過，如果已選取 [ **顯示所有活動的結果** ] (預設設定) 會傳回這些審計專案。</span><span class="sxs-lookup"><span data-stu-id="f2322-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="f2322-112">指定日期範圍，然後在 [ **使用者** ] 欄位中，選取您要調查之使用者的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="f2322-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="f2322-113">選取 [ **搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="f2322-113">Select **Search**.</span></span> <span data-ttu-id="f2322-114">活動會顯示在 [ **結果**] 底下。</span><span class="sxs-lookup"><span data-stu-id="f2322-114">The activities appear under **Results**.</span></span> <span data-ttu-id="f2322-115">您可以看到每個活動的 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="f2322-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="f2322-116">若要查看詳細資料，請選取活動，然後選取 [ **詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="f2322-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="f2322-117">若要深入瞭解，請參閱搜尋 [Office 365 audit log 以進行常見案例疑難排解](https://go.microsoft.com/fwlink/?linkid=2103944)。</span><span class="sxs-lookup"><span data-stu-id="f2322-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>