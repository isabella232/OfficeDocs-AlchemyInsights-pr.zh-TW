---
title: 'RBAC 角色 '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576430"
---
# <a name="rbac-rules"></a><span data-ttu-id="b84b1-102">RBAC 規則</span><span class="sxs-lookup"><span data-stu-id="b84b1-102">RBAC rules</span></span>

<span data-ttu-id="b84b1-103">如果您取得許可權錯誤：</span><span class="sxs-lookup"><span data-stu-id="b84b1-103">If you get the permission error:</span></span> 

- <span data-ttu-id="b84b1-104">**具有物件識別碼的用戶端未獲得透過範圍執行動作的授權 (程式碼： AuthorizationFailed)**：當您嘗試建立資源時，請檢查您目前是否已使用指派角色的使用者登入，該使用者具有選取範圍內的資源寫入權限。</span><span class="sxs-lookup"><span data-stu-id="b84b1-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="b84b1-105">例如，若要管理資源群組中的虛擬機器，您應該在資源群組 (或父項範圍) 上具有 [虛擬機器參與者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) 角色。</span><span class="sxs-lookup"><span data-stu-id="b84b1-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="b84b1-106">如需每個內建角色的許可權清單，請參閱 [Azure 資源的內建角色](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="b84b1-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="b84b1-107">**您沒有建立支援要求的許可權**：當您嘗試建立或更新支援票證時，請檢查您目前是否已被指派具有 Microsoft. 支援/supportTickets/寫入權限的使用者登入，例如 [支援要求參與者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)。</span><span class="sxs-lookup"><span data-stu-id="b84b1-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="b84b1-108">無法 **建立更多角色指派 (程式碼： RoleAssignmentLimitExceeded)**：當您嘗試指派角色時，請改為將角色指派給群組，以減少角色指派的數目。</span><span class="sxs-lookup"><span data-stu-id="b84b1-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="b84b1-109">Azure 每個訂閱最多可支援 **2000** 個角色指派。</span><span class="sxs-lookup"><span data-stu-id="b84b1-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="b84b1-110">如需 Azure RBAC 角色的詳細資訊，請參閱 [AZURE rbac role](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="b84b1-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
