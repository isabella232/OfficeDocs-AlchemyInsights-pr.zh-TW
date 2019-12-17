---
title: 效能問題 SharePoint 或 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068384"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="0dd6e-102">SharePoint 或 OneDrive 速度很慢，無法存取，或無法使用多個使用者</span><span class="sxs-lookup"><span data-stu-id="0dd6e-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="0dd6e-103">SharePoint 或 OneDrive 可能會變慢、 無法存取，或無法使用，或可能會顯示服務無法使用或 503 錯誤，幾個原因：</span><span class="sxs-lookup"><span data-stu-id="0dd6e-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="0dd6e-104">如果您的 SharePoint 或 OneDrive 網站緩慢或多個使用者延遲，可能有的暫時的服務問題： 使用者遇到間歇性延遲] 或 [瀏覽錯誤存取 SharePoint 網站或 OneDrive 內容時。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="0dd6e-105">檢查[服務健康狀況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)若要查看您的組織會受到影響。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="0dd6e-106">當您嘗試瀏覽至 SharePoint 或 OneDrive 網站時，使用者可能會收到*忙線 503 伺服器*的錯誤。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="0dd6e-107">此錯誤可能被因內 SharePoint 服務節流。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="0dd6e-108">SharePoint Online 使用節流以維持最佳的效能與可靠性的 SharePoint Online 服務。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="0dd6e-109">節流限制的使用者動作或並行數目 （來呼叫指令碼或程式碼） 以避免過度使用的資源。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="0dd6e-110">如需有關節流設定，請參閱[避免取得節流或封鎖 SharePoint Online 中](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="0dd6e-111">如果您遇到與**傳統**或**現代**的 SharePoint 網站或頁面的效能變慢，請利用[] 頁面上的診斷工具](https://aka.ms/perftool)來分析頁面。</span><span class="sxs-lookup"><span data-stu-id="0dd6e-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="0dd6e-112">如果您仍然一般效能變慢，請檢閱本文底部的資源：[效能調整 SharePoint Online 簡介](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="0dd6e-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  