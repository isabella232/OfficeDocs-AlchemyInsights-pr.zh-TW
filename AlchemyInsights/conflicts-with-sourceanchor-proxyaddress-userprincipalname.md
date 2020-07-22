---
title: 與 SourceAnchor、ProxyAddress、UserPrincipalName 衝突
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186105"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="ec5d3-102">與 SourceAnchor、ProxyAddress、UserPrincipalName 衝突</span><span class="sxs-lookup"><span data-stu-id="ec5d3-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="ec5d3-103">如果您在同步處理期間收到錯誤訊息，例如「目錄中存在相同 ProxyAddress 或 UserPrincipalName 的已同步處理物件」，請參閱[診斷和修正重複屬性同步處理錯誤](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors) (英文)。</span><span class="sxs-lookup"><span data-stu-id="ec5d3-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="ec5d3-104">此外，請考慮啟用重複屬性復原。</span><span class="sxs-lookup"><span data-stu-id="ec5d3-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="ec5d3-105">如需詳細資料，請參閱[身分識別同步處理及重複屬性復原](https://aka.ms/duplicateattributeresiliency) (英文)。</span><span class="sxs-lookup"><span data-stu-id="ec5d3-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>