---
title: 內容搜尋/匯出期間未傳回任何結果
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666642"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="5d596-102">內容搜尋/匯出期間未傳回任何結果</span><span class="sxs-lookup"><span data-stu-id="5d596-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="5d596-103">如果您在下列 eDiscovery 案例中遇到問題：</span><span class="sxs-lookup"><span data-stu-id="5d596-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="5d596-104">內容搜尋/匯出會傳回沒有資料或非預期的資料</span><span class="sxs-lookup"><span data-stu-id="5d596-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="5d596-105">eDiscovery 搜尋或匯出失敗</span><span class="sxs-lookup"><span data-stu-id="5d596-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="5d596-106">這可能是因為特定系統管理員所設定的某些相容性安全性篩選器所造成，但未傳遞給所有系統管理員。</span><span class="sxs-lookup"><span data-stu-id="5d596-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="5d596-107">若要解決此問題，請檢查是否有任何可能導致這些問題的相容性安全性篩選：</span><span class="sxs-lookup"><span data-stu-id="5d596-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="5d596-108">連接到安全性與合規性中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="5d596-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="5d596-109">執行下列 commandlets：</span><span class="sxs-lookup"><span data-stu-id="5d596-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="5d596-110">如需有關相容性安全性篩選的詳細資訊，請參閱 [內容搜尋的許可權篩選](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="5d596-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
