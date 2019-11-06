---
title: 2609 保留或 ediscovery 功能
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994048"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="11153-102">無法刪除 SharePoint Online 或商務用 OneDrive 中的項目</span><span class="sxs-lookup"><span data-stu-id="11153-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="11153-103">您或您的使用者可能無法刪除 SharePoint Online 中的項目或商務用 OneDrive 由於保留原則、 保留標籤或 eDiscovery 保留會套用至 SharePoint 的 OneDrive 網站或特定項目。</span><span class="sxs-lookup"><span data-stu-id="11153-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="11153-104">這包括無法刪除文件、 文件版本、 資料夾、 文件庫、 清單、 應用程式、 網站或網站集合。</span><span class="sxs-lookup"><span data-stu-id="11153-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="11153-105">以下是錯誤的一些郵件您可能會收到如果您嘗試刪除項目要保留訊息的範例：</span><span class="sxs-lookup"><span data-stu-id="11153-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="11153-106">「 因為它包含 eDiscovery 保留或保留原則中，無法刪除此網站 」</span><span class="sxs-lookup"><span data-stu-id="11153-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="11153-107">「 此網站含有合規性政策設定為封鎖刪除 」</span><span class="sxs-lookup"><span data-stu-id="11153-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="11153-108">「 合規性政策目前正在封鎖此刪除的網站 」</span><span class="sxs-lookup"><span data-stu-id="11153-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="11153-109">「 此網站集合無法被刪除，因為它包含 eDiscovery 保留或保留原則中包含的網站 」</span><span class="sxs-lookup"><span data-stu-id="11153-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="11153-110">「 您必須先刪除該資料夾刪除此資料夾中的所有項目 」</span><span class="sxs-lookup"><span data-stu-id="11153-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="11153-111">「 因為它是保留或保留原則上，無法刪除此項目的版本 」</span><span class="sxs-lookup"><span data-stu-id="11153-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="11153-112">「 無法在保留上刪除項目 」</span><span class="sxs-lookup"><span data-stu-id="11153-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="11153-113">"的標籤套用到這個項目，避免其成為編輯或刪除 」</span><span class="sxs-lookup"><span data-stu-id="11153-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="11153-114">「 清單無法保留或保留原則上刪除 」</span><span class="sxs-lookup"><span data-stu-id="11153-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="11153-115">「 如果就會封鎖作業，或保留原則套用至它，不能刪除清單 」</span><span class="sxs-lookup"><span data-stu-id="11153-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="11153-116">若要刪除這些案例中，保留原則、 保留標籤和 eDiscovery 的下列其中一項目保留已移除 （或網站有保留原則中排除）。</span><span class="sxs-lookup"><span data-stu-id="11153-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="11153-117">您要停用，或排除此問題所造成的個別保留。</span><span class="sxs-lookup"><span data-stu-id="11153-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="11153-118">會移除保留原則或保留之後，可能需要 24 小時的時間，變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="11153-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="11153-119">如需不同的保留和可套用至 SharePoint 網站與 OneDrive 帳戶的保留功能的相關資訊，請參閱下列主題。</span><span class="sxs-lookup"><span data-stu-id="11153-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="11153-120">保留原則概觀</span><span class="sxs-lookup"><span data-stu-id="11153-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="11153-121">保留標籤概觀</span><span class="sxs-lookup"><span data-stu-id="11153-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="11153-122">管理進階電子文件中的保留</span><span class="sxs-lookup"><span data-stu-id="11153-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="11153-123">eDiscovery 保留</span><span class="sxs-lookup"><span data-stu-id="11153-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="11153-124">舊版的網站關閉和刪除原則</span><span class="sxs-lookup"><span data-stu-id="11153-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
