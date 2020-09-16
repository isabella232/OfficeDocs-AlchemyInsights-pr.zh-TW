---
title: 單一使用者在 Outlook 中沒有看見增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719656"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="0db61-102">單一使用者在 Outlook 中沒有看見增益集</span><span class="sxs-lookup"><span data-stu-id="0db61-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="0db61-103">使用者可能屬於不具備正確 AppsForOfficeEnabled 參數的角色。</span><span class="sxs-lookup"><span data-stu-id="0db61-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="0db61-104">請執行此 Cmdlet，找出正確的角色是否與使用者相關聯：</span><span class="sxs-lookup"><span data-stu-id="0db61-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="0db61-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="0db61-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="0db61-106">如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。</span><span class="sxs-lookup"><span data-stu-id="0db61-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
