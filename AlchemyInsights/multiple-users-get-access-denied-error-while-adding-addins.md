---
title: 在 Outlook 中新增增益集時，多個使用者收到「拒絕存取」錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724354"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="14da8-102">在 Outlook 中新增增益集時，多個使用者收到「拒絕存取」錯誤</span><span class="sxs-lookup"><span data-stu-id="14da8-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="14da8-103">您可以指定組織中的哪些系統管理員具有安裝及管理 Outlook 增益集的權限。</span><span class="sxs-lookup"><span data-stu-id="14da8-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="14da8-104">您也可以指定組織中的哪些使用者有權限安裝及管理供其本身使用的增益集。</span><span class="sxs-lookup"><span data-stu-id="14da8-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="14da8-105">如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。</span><span class="sxs-lookup"><span data-stu-id="14da8-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="14da8-106">若要確認您已成功指派使用者的權限，請以要驗證的角色名稱取代 <Role Name>，然後在 Exchange Online PowerShell 中執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="14da8-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="14da8-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="14da8-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="14da8-108">此範例說明如何驗證您已指派給哪些人從組織的 Office 市集安裝增益集的權限。</span><span class="sxs-lookup"><span data-stu-id="14da8-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="14da8-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="14da8-109">PowerShell</span></span>

<span data-ttu-id="14da8-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="14da8-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="14da8-111">在 Get-ManagementRoleAssignment 的結果中，檢閱 [有效使用者] 欄中的項目。</span><span class="sxs-lookup"><span data-stu-id="14da8-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="14da8-112">如需詳細的語法和參數資訊，請參閱 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)。</span><span class="sxs-lookup"><span data-stu-id="14da8-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 