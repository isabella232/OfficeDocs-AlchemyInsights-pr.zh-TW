---
title: 疑難排解問題-在目錄中找不到使用者
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725398"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="03e95-102">疑難排解問題-在目錄中找不到使用者</span><span class="sxs-lookup"><span data-stu-id="03e95-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="03e95-103">如果使用者在目錄中收到錯誤訊息「找不到使用者」，請再試一次問題類型為使用者不在目錄中的地方。</span><span class="sxs-lookup"><span data-stu-id="03e95-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="03e95-104">您可以完成下列步驟以進行問題的疑難排解。</span><span class="sxs-lookup"><span data-stu-id="03e95-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="03e95-105">確定接受的電子郵件邀請的帳戶與以後用於登入的帳戶相同。</span><span class="sxs-lookup"><span data-stu-id="03e95-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="03e95-106">請確定使用者使用相同的帳戶來接受邀請並登入網站。</span><span class="sxs-lookup"><span data-stu-id="03e95-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="03e95-107">如需詳細資訊，請參閱 how [to </a> 365 manage](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)a a a a a a a a a a a a a a</span><span class="sxs-lookup"><span data-stu-id="03e95-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="03e95-108">流覽至使用者接收到錯誤的每個網站 (s) 。</span><span class="sxs-lookup"><span data-stu-id="03e95-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="03e95-109">在雙引號內新增 "/_layouts/15/people.aspx/membershipgroupid = 0" () 至網站 URL 的結尾。</span><span class="sxs-lookup"><span data-stu-id="03e95-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="03e95-110">範例： HTTPs://< "contoso" > sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。</span><span class="sxs-lookup"><span data-stu-id="03e95-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="03e95-111">從清單中選取使用者。</span><span class="sxs-lookup"><span data-stu-id="03e95-111">Select the user from the list.</span></span>

- <span data-ttu-id="03e95-112">按一下功能區中的 [ **移除使用者** 權力]。</span><span class="sxs-lookup"><span data-stu-id="03e95-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="03e95-113">新增回使用者，然後將邀請重新傳送給使用者。</span><span class="sxs-lookup"><span data-stu-id="03e95-113">Add back the User and Resend the invite to the user.</span></span>

