---
title: 單一使用者在 Outlook 中沒有看見增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154556"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="673d4-102">單一使用者在 Outlook 中沒有看見增益集</span><span class="sxs-lookup"><span data-stu-id="673d4-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="673d4-103">使用者可能屬於不具備正確 AppsForOfficeEnabled 參數的角色。</span><span class="sxs-lookup"><span data-stu-id="673d4-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="673d4-104">請執行此 Cmdlet，找出正確的角色是否與使用者相關聯：</span><span class="sxs-lookup"><span data-stu-id="673d4-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="673d4-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="673d4-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="673d4-106">如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。</span><span class="sxs-lookup"><span data-stu-id="673d4-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
