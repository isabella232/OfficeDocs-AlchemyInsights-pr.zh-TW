---
title: SharePoint Online 節流
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 5fdbb315698a58145e5437b0a7b127ce0062a76f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048607"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="eecc2-102">SharePoint Online 節流</span><span class="sxs-lookup"><span data-stu-id="eecc2-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="eecc2-103">使用者可能會收到 503 伺服器是忙碌錯誤，當您嘗試瀏覽至 SharePoint 或 OneDrive 網站時。</span><span class="sxs-lookup"><span data-stu-id="eecc2-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="eecc2-104">此錯誤可能被因內 SharePoint 服務節流。</span><span class="sxs-lookup"><span data-stu-id="eecc2-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="eecc2-105">SharePoint Online 使用節流以維持最佳的效能與可靠性的 SharePoint Online 服務。</span><span class="sxs-lookup"><span data-stu-id="eecc2-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="eecc2-106">節流限制的使用者動作或並行數目 （來呼叫指令碼或程式碼） 以避免過度使用的資源。</span><span class="sxs-lookup"><span data-stu-id="eecc2-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="eecc2-107">如果您不要取得節流，它是因為自訂程式碼的時間為 99%。</span><span class="sxs-lookup"><span data-stu-id="eecc2-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="eecc2-108">如需有關節流設定，請參閱[避免取得節流或封鎖 SharePoint Online 中](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="eecc2-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="eecc2-109">如果您認為這項錯誤，若要節流與無關，您可以檢查是否有發生在您的租用戶上由瀏覽至[訊息中心](https://portal.office.com/adminportal/home#/MessageCenter)的作用中維護。</span><span class="sxs-lookup"><span data-stu-id="eecc2-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="eecc2-110">最後，請確定您造訪 [[服務健康情況](https://portal.office.com/adminportal/home#/servicehealth)] 頁面上，若要檢查有可能會發生任何諮詢/事件。</span><span class="sxs-lookup"><span data-stu-id="eecc2-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

