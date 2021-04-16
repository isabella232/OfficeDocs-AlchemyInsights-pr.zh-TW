---
title: 在桌面機分析入職時，驗證存取權杖錯誤時發生錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813679"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="2fedb-102">在桌面分析上架時發生「驗證存取權杖時發生錯誤」錯誤</span><span class="sxs-lookup"><span data-stu-id="2fedb-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="2fedb-103">驗證權杖到期時，通常會觀測到此錯誤。</span><span class="sxs-lookup"><span data-stu-id="2fedb-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="2fedb-104">通常重新整理頁面會重新整理標記。</span><span class="sxs-lookup"><span data-stu-id="2fedb-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="2fedb-105">不過，如果有任何條件式存取原則套用至用來進行板載桌面機 Analytics 的帳戶，此問題便會存在。</span><span class="sxs-lookup"><span data-stu-id="2fedb-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="2fedb-106">您可以在 Azure 入口網站中檢查 Azure AD 登入記錄檔，以查看用於桌面機分析上架的帳戶是否有任何登入失敗。</span><span class="sxs-lookup"><span data-stu-id="2fedb-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="2fedb-107">如需條件式存取的相關資訊，請造訪 [規劃您的條件式存取部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。</span><span class="sxs-lookup"><span data-stu-id="2fedb-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>