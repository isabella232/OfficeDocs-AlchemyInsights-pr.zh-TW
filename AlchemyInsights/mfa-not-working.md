---
title: MFA 的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755122"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="de031-102">Azure MFA 的問題</span><span class="sxs-lookup"><span data-stu-id="de031-102">Issues with Azure MFA</span></span>
<span data-ttu-id="de031-103">有幾個事項可檢查使用者是否無法使用多重要素驗證 (MFA) 進行登入</span><span class="sxs-lookup"><span data-stu-id="de031-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="de031-104">受影響的使用者可能會在 Azure Active Directory 入口網站中封鎖。</span><span class="sxs-lookup"><span data-stu-id="de031-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="de031-105">如果是這種情況，該特定使用者的驗證嘗試將會自動遭到拒絕。</span><span class="sxs-lookup"><span data-stu-id="de031-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="de031-106">請依照本文中的步驟加以取消封鎖。</span><span class="sxs-lookup"><span data-stu-id="de031-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="de031-107">如果解除封鎖使用者沒有説明，或使用者未封鎖，您可以嘗試為使用者重設 MFA，然後再次進行註冊程式。</span><span class="sxs-lookup"><span data-stu-id="de031-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="de031-108">請依照本文中的步驟進行。</span><span class="sxs-lookup"><span data-stu-id="de031-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="de031-109">如果這是您第一次啟用 MFA，而且使用者無法登入非瀏覽器用戶端（例如 Outlook、Skype 等等），則您的 O365 訂閱上沒有啟用該 (Active Directory 驗證程式庫) 。</span><span class="sxs-lookup"><span data-stu-id="de031-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="de031-110">在此情況下，您將需要連線到 Exchange Online Powershell，並執行此 Cmdlet：  *Set-OrganizationConfig-OAuth2ClientProfileEnabled： $true*</span><span class="sxs-lookup"><span data-stu-id="de031-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>