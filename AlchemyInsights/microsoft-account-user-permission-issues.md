---
title: 疑難排解問題-目錄中找不到使用者
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249904"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="b0eb1-102">疑難排解問題-目錄中找不到使用者</span><span class="sxs-lookup"><span data-stu-id="b0eb1-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="b0eb1-103">如果使用者會收到錯誤訊息 「 使用者找不到 」 目錄中。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="b0eb1-104">請再試一次其中問題類型是使用者不在目錄中。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="b0eb1-105">若要疑難排解問題，可以完成下列步驟。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="b0eb1-106">確定公認的電子郵件邀請是相同的帳戶是用來以稍後再登入的帳戶。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="b0eb1-107">請確定使用者以接受邀請，並登入網站使用相同的帳戶。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="b0eb1-108">如需詳細資訊，請參閱[如何管理您的 Microsoft 帳戶的別名</a>來管理 Office 365 登入](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="b0eb1-109">瀏覽至每個網站中的使用者會收到錯誤。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="b0eb1-110">新增 「 / _layouts/15/people.aspx/membershipgroupid=0 」 （內雙引號） 的網站 URL 的結尾。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="b0eb1-111">範例： https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="b0eb1-112">從清單中選取使用者。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-112">Select the user from the list.</span></span>

- <span data-ttu-id="b0eb1-113">按一下 [從功能區的 [**移除使用者權限**。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="b0eb1-114">將使用者新增回並重新邀請傳送給使用者。</span><span class="sxs-lookup"><span data-stu-id="b0eb1-114">Add back the User and Resend the invite to the user.</span></span>

