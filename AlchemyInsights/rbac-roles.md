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
# <a name="rbac-rules"></a>RBAC 規則

如果您取得許可權錯誤： 

- **具有物件識別碼的用戶端未獲得透過範圍執行動作的授權 (程式碼： AuthorizationFailed)**：當您嘗試建立資源時，請檢查您目前是否已使用指派角色的使用者登入，該使用者具有選取範圍內的資源寫入權限。 例如，若要管理資源群組中的虛擬機器，您應該在資源群組 (或父項範圍) 上具有 [虛擬機器參與者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) 角色。 如需每個內建角色的許可權清單，請參閱 [Azure 資源的內建角色](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)。
- **您沒有建立支援要求的許可權**：當您嘗試建立或更新支援票證時，請檢查您目前是否已被指派具有 Microsoft. 支援/supportTickets/寫入權限的使用者登入，例如 [支援要求參與者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)。
- 無法 **建立更多角色指派 (程式碼： RoleAssignmentLimitExceeded)**：當您嘗試指派角色時，請改為將角色指派給群組，以減少角色指派的數目。 Azure 每個訂閱最多可支援 **2000** 個角色指派。

如需 Azure RBAC 角色的詳細資訊，請參閱 [AZURE rbac role](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。
