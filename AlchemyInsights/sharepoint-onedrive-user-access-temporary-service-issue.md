---
title: SharePoint 或 OneDrive 效能問題
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719508"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="2d65a-102">SharePoint 或 OneDrive 變慢、無法存取或無法多名使用者使用</span><span class="sxs-lookup"><span data-stu-id="2d65a-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="2d65a-103">如果以前具有存取權限的多名使用者現在無法使用 OneDrive 或 SharePoint 網站，則可能有暫時服務的問題。</span><span class="sxs-lookup"><span data-stu-id="2d65a-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="2d65a-104">[請查看服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="2d65a-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="2d65a-105">新增及授權使用者</span><span class="sxs-lookup"><span data-stu-id="2d65a-105">Add and license the user</span></span>

<span data-ttu-id="2d65a-106">確定[在商務用 Office 365 中指派授權給使用者](https://docs.microsoft.com/zh-TW/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)。</span><span class="sxs-lookup"><span data-stu-id="2d65a-106">[Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="2d65a-107">指派權限</span><span class="sxs-lookup"><span data-stu-id="2d65a-107">Assign permissions</span></span>

<span data-ttu-id="2d65a-108">如果已指派使用者 Sharepoint 授權，但還是收到拒絕存取的訊息，請確定有[指派使用者適當層級](https://docs.microsoft.com/zh-TW/sharepoint/understanding-permission-levels)的權限。</span><span class="sxs-lookup"><span data-stu-id="2d65a-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="2d65a-109">請考慮使用存取要求功能</span><span class="sxs-lookup"><span data-stu-id="2d65a-109">Consider using the access request feature</span></span>

<span data-ttu-id="2d65a-110">
  [存取 ](https://support.office.com/zh-TW/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)要求功能可讓使用者要求存取他們目前無權查看的內容。</span><span class="sxs-lookup"><span data-stu-id="2d65a-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="2d65a-111">允許自訂指令碼可能會造成拒絕存取的問題</span><span class="sxs-lookup"><span data-stu-id="2d65a-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="2d65a-112">某些情況下，*允許自訂指令碼*功能可能會顯示拒絕存取。</span><span class="sxs-lookup"><span data-stu-id="2d65a-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="2d65a-113">如需受影響功能清單、安全性考量，以及停用此功能的能力。</span><span class="sxs-lookup"><span data-stu-id="2d65a-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="2d65a-114">請參閱[允許或防止自訂指令碼 (機器翻譯)](https://docs.microsoft.com/zh-TW/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="2d65a-114">[Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

