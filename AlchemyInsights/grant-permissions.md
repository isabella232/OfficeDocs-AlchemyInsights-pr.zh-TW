---
title: 授與權限
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897699"
---
# <a name="grant-permissions"></a><span data-ttu-id="8484c-102">授與權限</span><span class="sxs-lookup"><span data-stu-id="8484c-102">Grant permissions</span></span>

1. <span data-ttu-id="8484c-103">授 **與租** 使用者系統管理員的同意：請參閱 [授與租](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)使用者系統管理員同意的逐步指示，以授與受租使用者管理員同意之 azure 入口網站、使用 azure AD PowerShell，或從同意提示自身。</span><span class="sxs-lookup"><span data-stu-id="8484c-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="8484c-104">**代表特定使用者授與同意**：不是授與整個組織的同意，管理員也可以使用 [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) 來代表單一使用者授與委派許可權。</span><span class="sxs-lookup"><span data-stu-id="8484c-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="8484c-105">如需詳細資訊，請參閱 [代表使用者取得存取權](https://docs.microsoft.com/graph/auth-v2-user)。</span><span class="sxs-lookup"><span data-stu-id="8484c-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>