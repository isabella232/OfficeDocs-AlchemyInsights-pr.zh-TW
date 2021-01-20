---
title: 登出問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886799"
---
# <a name="sign-out-issues"></a><span data-ttu-id="27da4-102">登出問題</span><span class="sxs-lookup"><span data-stu-id="27da4-102">Sign-out issues</span></span>

<span data-ttu-id="27da4-103">若要解決與登出相關的問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="27da4-103">To resolve issues related to signing out, perform the following steps:</span></span>

1. <span data-ttu-id="27da4-104">如果應用程式正在紀錄或將您或使用者登出應用程式，請依照文章 [使用條件式存取設定驗證會話管理](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) 或 [在 [適用於開發人員的 Microsoft 身分識別平台] 設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 的指引。</span><span class="sxs-lookup"><span data-stu-id="27da4-104">If you or a user are getting logged or kicked out of applications, follow the guidance in the articles [Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) or [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="27da4-105">藉由疑難排解 Azure Active Directory (Azure AD) 與特定應用程式的整合，就能解決大多數的其他登入錯誤或問題。</span><span class="sxs-lookup"><span data-stu-id="27da4-105">Most other sign-out errors or problems can be solved by troubleshooting the integration of Azure Active Directory (Azure AD) with the specific application.</span></span> <span data-ttu-id="27da4-106">您可以尋找特定整合的指導方針，只需移至此 [教學課程集合，以便將應用程式與 Azure Active Directory 整合](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)，包括：</span><span class="sxs-lookup"><span data-stu-id="27da4-106">You can find guidance for a specific integration by going to this [collection of tutorials for integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list), including:</span></span>
    - <span data-ttu-id="27da4-107">SaaS 應用程式教學課程</span><span class="sxs-lookup"><span data-stu-id="27da4-107">SaaS application tutorials</span></span>
    - <span data-ttu-id="27da4-108">單一登入教學課程</span><span class="sxs-lookup"><span data-stu-id="27da4-108">Single sign-on tutorials</span></span>
    - <span data-ttu-id="27da4-109">使用者佈建教學課程</span><span class="sxs-lookup"><span data-stu-id="27da4-109">User-provisioning tutorials</span></span>