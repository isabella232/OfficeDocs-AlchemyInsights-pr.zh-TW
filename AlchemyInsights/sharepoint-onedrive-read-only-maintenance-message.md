---
title: 嘗試使用 SharePoint 或 OneDrive 時進行維護訊息的 Read-Only
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670823"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="8fad5-102">嘗試使用 SharePoint 或 OneDrive 時進行維護訊息的 Read-Only</span><span class="sxs-lookup"><span data-stu-id="8fad5-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="8fad5-103">當下列其中一種案例嘗試使用 SharePoint 或 OneDrive 時，使用者可能會收到 **Read-Only 以進行維護** 訊息。</span><span class="sxs-lookup"><span data-stu-id="8fad5-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="8fad5-104">已計畫或主動維護活動。</span><span class="sxs-lookup"><span data-stu-id="8fad5-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="8fad5-105">流覽至 [訊息中心](https://portal.office.com/adminportal/home#/messagecenter)以檢查是否有這些檔案。</span><span class="sxs-lookup"><span data-stu-id="8fad5-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="8fad5-106">可能發生的高優先順序主動服務事件。</span><span class="sxs-lookup"><span data-stu-id="8fad5-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="8fad5-107">流覽至 [服務健康情況](https://portal.office.com/adminportal/home#/servicehealth)，以檢查是否有任何建議/事件。</span><span class="sxs-lookup"><span data-stu-id="8fad5-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="8fad5-108">一種次要的自動修復復原案例，因為伺服器上可能有超過30分鐘以上的任何未預期事件，可能會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="8fad5-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="8fad5-109">這些次要復原沒有任何訊息中心或服務健康情況文章，但您應該可以立即恢復正常。</span><span class="sxs-lookup"><span data-stu-id="8fad5-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="8fad5-110">在極少數的情況下，我們看到上述三個案例中的其中一種是導致原因，而服務已還原，但使用者瀏覽器快取尚未清除。</span><span class="sxs-lookup"><span data-stu-id="8fad5-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="8fad5-111">請先嘗試清除瀏覽器快取，然後再流覽至網站。</span><span class="sxs-lookup"><span data-stu-id="8fad5-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="8fad5-112">在您的 Microsoft Edge browser 中，選取 [ **設定**]，然後選取 [ **隱私權與安全性**]。</span><span class="sxs-lookup"><span data-stu-id="8fad5-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="8fad5-113">在 [ **清除流覽**] 底下，選取 **[選擇要清除**的專案]。</span><span class="sxs-lookup"><span data-stu-id="8fad5-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="8fad5-114">選取 [ **cookie] 和 [儲存的網站資料**]，然後選取 [ **清除**]。</span><span class="sxs-lookup"><span data-stu-id="8fad5-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="8fad5-115">當您使用其他瀏覽器（例如 Mozilla Firefox 或 Google Chrome）時，可能會有不同的步驟。</span><span class="sxs-lookup"><span data-stu-id="8fad5-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="8fad5-116">另一個選項是在新的 InPrivate 視窗中開啟 SharePoint 網站或 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="8fad5-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>