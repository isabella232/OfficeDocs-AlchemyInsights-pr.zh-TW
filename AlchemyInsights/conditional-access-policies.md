---
title: 條件式存取原則
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100411"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="4175f-102">條件式存取原則</span><span class="sxs-lookup"><span data-stu-id="4175f-102">Conditional Access policies</span></span>

<span data-ttu-id="4175f-103">條件式存取是 Azure AD 的一項功能，可讓您強制控制環境中應用程式的存取，而這一切都是根據特定條件，並由中央位置所管理。</span><span class="sxs-lookup"><span data-stu-id="4175f-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="4175f-104">深入了解 [Azure AD 條件式存取](https://docs.microsoft.com/azure/active-directory/conditional-access/)。</span><span class="sxs-lookup"><span data-stu-id="4175f-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="4175f-105">**注意**: 如果您的租用戶是在 2019 年 10 月 21 日之後建立，且意外收到 MFA 的提示，則可能已在租用戶中啟用[安全性預設](http://aka.ms/securitydefaults)。</span><span class="sxs-lookup"><span data-stu-id="4175f-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="4175f-106">**若要管理安全性預設**</span><span class="sxs-lookup"><span data-stu-id="4175f-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="4175f-107">使用全域系統管理員認證登入[系統管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822)。</span><span class="sxs-lookup"><span data-stu-id="4175f-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="4175f-108">移至 [Azure Active Directory 屬性](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)。</span><span class="sxs-lookup"><span data-stu-id="4175f-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="4175f-109">在頁面底部，按一下 [管理安全性預設]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="4175f-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="4175f-110">按一下 **[是]** 啟用安全性預設，或 **[否]** 停用安全性預設。</span><span class="sxs-lookup"><span data-stu-id="4175f-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
