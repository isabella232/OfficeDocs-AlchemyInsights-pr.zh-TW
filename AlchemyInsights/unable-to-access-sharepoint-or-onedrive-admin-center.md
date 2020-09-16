---
title: 無法存取 SharePoint 或 OneDrive 系統管理中心
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: a70b0708b325c5feaefec3d97c957086d7f62cc6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749469"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="db4b8-102">無法存取 SharePoint 或 OneDrive 系統管理中心</span><span class="sxs-lookup"><span data-stu-id="db4b8-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="db4b8-103">如果您的 SharePoint 或 OneDrive 系統管理中心網站無法存取或無法使用，可能發生暫時的服務問題，即使用者在存取 SharePoint 網站或 OneDrive 內容時遇到間歇性延遲或導覽錯誤。</span><span class="sxs-lookup"><span data-stu-id="db4b8-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="db4b8-104">請查看[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解您的組織是否受到影響。</span><span class="sxs-lookup"><span data-stu-id="db4b8-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="db4b8-105">您必須將 SharePoint 授權指派給全域和 SharePoint 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="db4b8-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="db4b8-106">剛使用 SharePoint 授權或系統管理員角色指派的新建帳戶，可能會在存取 SharePoint 時遇到問題，例如「拒絕存取」或「找不到使用者」。</span><span class="sxs-lookup"><span data-stu-id="db4b8-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="db4b8-107">請至少等候 24 小時，以完成整個系統的同步處理。</span><span class="sxs-lookup"><span data-stu-id="db4b8-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="db4b8-108">我們知道 24 小時可能感覺有點久。</span><span class="sxs-lookup"><span data-stu-id="db4b8-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="db4b8-109">多數情況下，我們已經著手研究解決方案。</span><span class="sxs-lookup"><span data-stu-id="db4b8-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="db4b8-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) 如果允許非常短的存取時間，使用者可能會收到拒絕存取，請參閱[拒絕存取 PIM 帳戶](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)。</span><span class="sxs-lookup"><span data-stu-id="db4b8-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>