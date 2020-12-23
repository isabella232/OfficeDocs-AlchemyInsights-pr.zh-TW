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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727214"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="19d7b-102">內容搜尋/匯出期間未傳回任何結果</span><span class="sxs-lookup"><span data-stu-id="19d7b-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="19d7b-103">如果您在下列 eDiscovery 案例中遇到問題：</span><span class="sxs-lookup"><span data-stu-id="19d7b-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="19d7b-104">內容搜尋/匯出會傳回沒有資料或非預期的資料</span><span class="sxs-lookup"><span data-stu-id="19d7b-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="19d7b-105">eDiscovery 搜尋或匯出失敗</span><span class="sxs-lookup"><span data-stu-id="19d7b-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="19d7b-106">這可能是因為特定系統管理員所設定的某些規範安全性篩選器，但未傳遞給所有系統管理員。</span><span class="sxs-lookup"><span data-stu-id="19d7b-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="19d7b-107">若要解決此問題，請檢查是否有任何可能導致這些問題的相容性安全性篩選：</span><span class="sxs-lookup"><span data-stu-id="19d7b-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="19d7b-108">連接到安全性與合規性中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="19d7b-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="19d7b-109">執行下列 commandlets：</span><span class="sxs-lookup"><span data-stu-id="19d7b-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="19d7b-110">如需有關相容性安全性篩選的詳細資訊，請參閱 [內容搜尋的許可權篩選](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="19d7b-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
