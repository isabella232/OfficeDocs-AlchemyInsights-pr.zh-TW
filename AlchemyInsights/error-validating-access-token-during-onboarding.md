---
title: 在桌面分析登入期間驗證存取 token 錯誤時發生錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741130"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="a6f2a-102">桌面分析上架期間 」 時發生錯誤驗證存取權杖 」 錯誤</span><span class="sxs-lookup"><span data-stu-id="a6f2a-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="a6f2a-103">此錯誤通常是觀察到的驗證權杖到期時。</span><span class="sxs-lookup"><span data-stu-id="a6f2a-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="a6f2a-104">通常，重新整理頁面重新整理權杖。</span><span class="sxs-lookup"><span data-stu-id="a6f2a-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="a6f2a-105">不過，這個問題可以保存如果沒有任何條件式存取原則套用至所使用的帳戶到委任桌面分析。</span><span class="sxs-lookup"><span data-stu-id="a6f2a-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="a6f2a-106">您可以檢閱 [Azure AD 登入 Azure 入口網站中的記錄檔中是否有任何登入失敗的桌面分析上架所使用的帳戶。</span><span class="sxs-lookup"><span data-stu-id="a6f2a-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="a6f2a-107">如需條件式存取的詳細資訊，請瀏覽[規劃條件式存取部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。</span><span class="sxs-lookup"><span data-stu-id="a6f2a-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>