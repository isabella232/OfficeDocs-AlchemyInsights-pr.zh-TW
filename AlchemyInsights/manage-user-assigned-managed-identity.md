---
title: 管理使用者指派的受控身分識別
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177301"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="1b0a6-102">管理使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="1b0a6-103">使用者指派的受控身分識別管理包括：</span><span class="sxs-lookup"><span data-stu-id="1b0a6-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="1b0a6-104">將角色指派給使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="1b0a6-105">刪除使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="1b0a6-106">列出使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="1b0a6-107">如需上述工作的詳細資訊，請參閱下列文章：</span><span class="sxs-lookup"><span data-stu-id="1b0a6-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="1b0a6-108">[如何建立使用者指派的受控身分識別](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - 用於指派角色給使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="1b0a6-109">[如何刪除使用者指派的受控身分識別](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - 用於刪除使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="1b0a6-110">[如何列出使用者指派的受控身分識別](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - 用於列出使用者指派的受控身分識別</span><span class="sxs-lookup"><span data-stu-id="1b0a6-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="1b0a6-111">驗證您是否擁有 **受控身分識別參與者** 角色指派。</span><span class="sxs-lookup"><span data-stu-id="1b0a6-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="1b0a6-112">該角色指派需建立/刪除使用者指派的受控身分識別。</span><span class="sxs-lookup"><span data-stu-id="1b0a6-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
