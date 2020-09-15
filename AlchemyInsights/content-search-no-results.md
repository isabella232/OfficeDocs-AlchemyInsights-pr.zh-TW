---
title: 沒有結果的內容搜尋
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680638"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="7c25a-102">內容搜尋/匯出沒有任何結果</span><span class="sxs-lookup"><span data-stu-id="7c25a-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="7c25a-103">內容搜尋/匯出的問題未傳回任何資料可能是由於特定系統管理員所設定的某些規範安全性篩選，但未與所有系統管理員通訊。</span><span class="sxs-lookup"><span data-stu-id="7c25a-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="7c25a-104">若要解決此問題，請查看是否有任何可能導致問題的相容性安全性篩選：</span><span class="sxs-lookup"><span data-stu-id="7c25a-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="7c25a-105">連接到安全性與合規性中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="7c25a-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="7c25a-106">執行下列 commandlets：</span><span class="sxs-lookup"><span data-stu-id="7c25a-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="7c25a-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="7c25a-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="7c25a-108">Remove-compliancesecurityfilter-組織 $org</span><span class="sxs-lookup"><span data-stu-id="7c25a-108">Get-ComplianceSecurityFilter -Organization $org</span></span>