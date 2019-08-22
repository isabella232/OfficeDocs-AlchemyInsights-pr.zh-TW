---
title: 內容搜尋任何結果
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516770"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="32860-102">從內容搜尋/匯出任何結果</span><span class="sxs-lookup"><span data-stu-id="32860-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="32860-103">問題使用內容搜尋/匯出不傳回任何資料可能會因為某些法規安全性篩選器所安裝的特定的系統管理員並沒有通訊用於所有的系統管理員。</span><span class="sxs-lookup"><span data-stu-id="32860-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="32860-104">若要解決此問題，請檢查是否有可能原因包括下列任何法規安全性篩選器：</span><span class="sxs-lookup"><span data-stu-id="32860-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="32860-105">連接到安全性與合規性中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="32860-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="32860-106">執行下列 commandlets:</span><span class="sxs-lookup"><span data-stu-id="32860-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="32860-107">$org ="yourdomain.com 」</span><span class="sxs-lookup"><span data-stu-id="32860-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="32860-108">取得 ComplianceSecurityFilter-組織 $org</span><span class="sxs-lookup"><span data-stu-id="32860-108">Get-ComplianceSecurityFilter -Organization $org</span></span>