---
title: 解決 Teams 登入錯誤 AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2020
ms.locfileid: "44328786"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="d2526-102">解決 Teams 登入錯誤 AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="d2526-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="d2526-103">當登入 Microsoft Teams 時，您可能會收到以下錯誤：[很抱歉，我們無法將您登入 AADSTS9000411: 要求的格式不正確。參數 "login_hint" 重複。]\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="d2526-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="d2526-104">若要解決此問題，請確認您的 Microsoft Teams 用戶端已更新。</span><span class="sxs-lookup"><span data-stu-id="d2526-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="d2526-105">如需更新用戶端的詳細資訊，請參閱[更新 Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="d2526-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="d2526-106">如果您因為某些原因而無法更新用戶端，登出用戶端將清除大部分的快取資料。</span><span class="sxs-lookup"><span data-stu-id="d2526-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="d2526-107">不過，如果您在登出/登入後仍有問題，請結束 Teams，並執行下列動作清除用戶端快取：</span><span class="sxs-lookup"><span data-stu-id="d2526-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="d2526-108">關閉 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="d2526-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="d2526-109">移至：%appdata%\microsoft\teams 並刪除所有檔案。</span><span class="sxs-lookup"><span data-stu-id="d2526-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="d2526-110">重新開啟 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="d2526-110">Reopen Microsoft Teams.</span></span>
