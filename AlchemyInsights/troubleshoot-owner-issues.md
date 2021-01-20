---
title: 疑難排解擁有者問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886797"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="cebbf-102">疑難排解擁有者問題</span><span class="sxs-lookup"><span data-stu-id="cebbf-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="cebbf-103">若要疑難排解擁有者相關問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="cebbf-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="cebbf-104">[新增或變更 Azure 訂閱系統管理員](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)： Azure Active Directory (Azure AD) 群組為群組擁有者擁有和管理。</span><span class="sxs-lookup"><span data-stu-id="cebbf-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="cebbf-105">群組擁有者可以是使用者或服務主體，且能夠管理群組，包括成員資格。</span><span class="sxs-lookup"><span data-stu-id="cebbf-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="cebbf-106">只有現有的群組擁有者或群組管理系統管理員可以指派群組擁有者。</span><span class="sxs-lookup"><span data-stu-id="cebbf-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="cebbf-107">群組擁有者不一定要是該群組的成員。</span><span class="sxs-lookup"><span data-stu-id="cebbf-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="cebbf-108">[新增或變更 Azure 訂閱系統管理員](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)：本文說明如何在訂閱範圍中使用 Azure RBAC 新增或變更使用者的系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="cebbf-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="cebbf-109">使用 PowerShell 以新增群組擁有者或應用程式擁有者。</span><span class="sxs-lookup"><span data-stu-id="cebbf-109">Use PowerShell to add a group owner or an application owner.</span></span>
