---
title: 針對共用原則與組織關聯性使用 PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826046"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>針對共用原則與組織關聯性使用 PowerShell


對於組織關聯性，請檢閱以下各項的詳細語法和參數資訊：[Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)、[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)、[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) 和 [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)。

若要建立共用原則，請使用 [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)。 若要[將共用原則套用至信箱或使用者](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)，您需要對新建立的原則使用 [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) 和 [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) 的組合。 若要[修改、停用或移除共用原則](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)，您需要使用 [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) 和 [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)。

**如需深入了解本主題，請參閱：**

[在 Exchange Online 中共用](https://docs.microsoft.com/exchange/sharing/sharing)