---
title: 還原已刪除的 Microsoft 365 群組
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645122"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="feec3-102">還原已刪除的 Microsoft 365 群組</span><span class="sxs-lookup"><span data-stu-id="feec3-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="feec3-103">您可以從刪除的30天內，還原已刪除的 Microsoft 365 群組或 Microsoft 團隊。</span><span class="sxs-lookup"><span data-stu-id="feec3-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="feec3-104">移至 [Microsoft 365 系統管理中心](https://aka.ms/RestoreDeletedGroup) ，登入您已刪除的群組和小組清單。</span><span class="sxs-lookup"><span data-stu-id="feec3-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="feec3-105">**附注：** 使用指派給承租人管理員或群組管理員角色的帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="feec3-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="feec3-106">選取要還原的 [已刪除的 Microsoft 365 群組/小組]，然後按一下 [ **還原群組**]。</span><span class="sxs-lookup"><span data-stu-id="feec3-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="feec3-107">若由於 SMTP 位址衝突而無法還原群組，請使用下列命令來找出導致衝突的物件，並移除 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="feec3-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="feec3-108">**附注：** 在某些情況下，您可能需要24小時的時間才能還原群組及其所有資料。</span><span class="sxs-lookup"><span data-stu-id="feec3-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="feec3-109">如需詳細資訊，或若要瞭解如何使用 PowerShell 還原群組，請參閱 [還原已刪除的 Microsoft 365 群組](https://go.microsoft.com/fwlink/?linkid=867802)。</span><span class="sxs-lookup"><span data-stu-id="feec3-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>