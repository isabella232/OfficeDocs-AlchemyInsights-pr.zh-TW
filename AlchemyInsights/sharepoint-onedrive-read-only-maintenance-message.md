---
title: 唯讀的維護郵件時嘗試使用 SharePoint 或 OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620714"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="9889f-102">唯讀的維護郵件時嘗試使用 SharePoint 或 OneDrive</span><span class="sxs-lookup"><span data-stu-id="9889f-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="9889f-103">當您嘗試使用下列其中一個下列案例 SharePoint 或 OneDrive 時，使用者可能會收到**唯讀維護的**郵件。</span><span class="sxs-lookup"><span data-stu-id="9889f-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="9889f-104">計劃或作用中的維護活動。</span><span class="sxs-lookup"><span data-stu-id="9889f-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="9889f-105">檢查其瀏覽至[訊息中心](https://portal.office.com/adminportal/home#/messagecenter)。</span><span class="sxs-lookup"><span data-stu-id="9889f-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="9889f-106">高優先順序 active 服務事件，可能會發生。</span><span class="sxs-lookup"><span data-stu-id="9889f-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="9889f-107">瀏覽至[服務健康情況](https://portal.office.com/adminportal/home#/servicehealth)檢查任何諮詢/事件。</span><span class="sxs-lookup"><span data-stu-id="9889f-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="9889f-108">次要自動修復復原案例中，就可能發生由於任何未預期的事件可能會持續小於 30 分鐘或操作的伺服器上。</span><span class="sxs-lookup"><span data-stu-id="9889f-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="9889f-109">有無訊息中心或服務健康情況文章，這些次要復原，但您應為 [正常很快。</span><span class="sxs-lookup"><span data-stu-id="9889f-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="9889f-110">在極少情況下我們觀察到上述的三個案例的其中一個已原因，和已還原服務，但使用者瀏覽器快取尚未被清除。</span><span class="sxs-lookup"><span data-stu-id="9889f-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="9889f-111">請嘗試瀏覽至網站之前，清除瀏覽器快取。</span><span class="sxs-lookup"><span data-stu-id="9889f-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="9889f-112">在您在 Microsoft Edge 瀏覽器中，選取 [**設定**]，然後選取**隱私及安全性**。</span><span class="sxs-lookup"><span data-stu-id="9889f-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="9889f-113">在**清除瀏覽**，選取 [**選擇要清除項目**。</span><span class="sxs-lookup"><span data-stu-id="9889f-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="9889f-114">選取 [ **Cookie 和儲存的網站資料**]，然後選取 [**清除**。</span><span class="sxs-lookup"><span data-stu-id="9889f-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="9889f-115">使用 Mozilla Firefox 或 Google Chrome 等其他瀏覽器時，這些步驟可能會不同。</span><span class="sxs-lookup"><span data-stu-id="9889f-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="9889f-116">另一個方式則是在新的 InPrivate 視窗中開啟您的 SharePoint 網站或 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="9889f-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>