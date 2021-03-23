---
title: 關於 Yammer 系統管理員
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995244"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="4bf16-102">關於 Yammer 系統管理員</span><span class="sxs-lookup"><span data-stu-id="4bf16-102">About Yammer admins</span></span>

<span data-ttu-id="4bf16-103">**網路系統管理員**</span><span class="sxs-lookup"><span data-stu-id="4bf16-103">**Network admins**</span></span>

<span data-ttu-id="4bf16-104">全域管理員會自動升級為 Yammer 網路中已驗證的系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="4bf16-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="4bf16-105">在下列情況下，此升級可能無法正確進行：</span><span class="sxs-lookup"><span data-stu-id="4bf16-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="4bf16-106">有多個 Yammer 網路存在，且系統管理員已登入錯誤的網路。</span><span class="sxs-lookup"><span data-stu-id="4bf16-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="4bf16-107">若要取得一個 Yammer 網路，需要進行[網路整合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)。</span><span class="sxs-lookup"><span data-stu-id="4bf16-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="4bf16-108">使用 Azure PIM。</span><span class="sxs-lookup"><span data-stu-id="4bf16-108">Azure PIM is being used.</span></span> <span data-ttu-id="4bf16-109">使用者可能不會提升為全域系統管理員足夠長的時間來進行升級。</span><span class="sxs-lookup"><span data-stu-id="4bf16-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="4bf16-110">後續的 Yammer 更新可能會解決此問題，但最好是手動將使用者提升為全域管理員。</span><span class="sxs-lookup"><span data-stu-id="4bf16-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="4bf16-111">Yammer 網路存在同步處理問題。</span><span class="sxs-lookup"><span data-stu-id="4bf16-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="4bf16-112">在此情況下，將需要支援要求才能進行進一步調查。</span><span class="sxs-lookup"><span data-stu-id="4bf16-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="4bf16-113">如需 Yammer 系統管理員角色的詳細資訊，請參閱 [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)。</span><span class="sxs-lookup"><span data-stu-id="4bf16-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="4bf16-114">**群組管理員**</span><span class="sxs-lookup"><span data-stu-id="4bf16-114">**Group admins**</span></span>

<span data-ttu-id="4bf16-115">Microsoft 365 連接的群組的群組管理員會與 Azure AD 中的群組成員資格同步處理。</span><span class="sxs-lookup"><span data-stu-id="4bf16-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="4bf16-116">若為大型群組，此同步處理可能需要較長的期限。</span><span class="sxs-lookup"><span data-stu-id="4bf16-116">For large groups, this sync can take an extended period.</span></span>
