---
title: 針對共用原則與組織關聯性使用 PowerShell
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
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709457"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="bfd21-102">針對共用原則與組織關聯性使用 PowerShell</span><span class="sxs-lookup"><span data-stu-id="bfd21-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="bfd21-103">對於組織關聯性，請檢閱以下各項的詳細語法和參數資訊：[Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)、[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)、[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) 和 [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)。</span><span class="sxs-lookup"><span data-stu-id="bfd21-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="bfd21-104">若要建立共用原則，請使用 [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)。</span><span class="sxs-lookup"><span data-stu-id="bfd21-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="bfd21-105">若要[將共用原則套用至信箱或使用者](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)，您需要對新建立的原則使用 [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) 和 [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) 的組合。</span><span class="sxs-lookup"><span data-stu-id="bfd21-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="bfd21-106">若要[修改、停用或移除共用原則](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)，您需要使用 [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) 和 [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)。</span><span class="sxs-lookup"><span data-stu-id="bfd21-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="bfd21-107">**如需深入了解本主題，請參閱：**</span><span class="sxs-lookup"><span data-stu-id="bfd21-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="bfd21-108">在 Exchange Online 中共用</span><span class="sxs-lookup"><span data-stu-id="bfd21-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)