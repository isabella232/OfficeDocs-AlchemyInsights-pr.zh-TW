---
title: 使用者收到錯誤 AADSTS7000112 Yammer 已停用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796639"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="ba585-102">使用者收到錯誤 AADSTS7000112 Yammer 已停用</span><span class="sxs-lookup"><span data-stu-id="ba585-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="ba585-103">如果您收到「AADSTS7000112： Application ' 00000005-0000-0ff1-ce00-000000000000 ' （Yammer）」錯誤，則表示 Azure AD 中的服務主體有問題。</span><span class="sxs-lookup"><span data-stu-id="ba585-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="ba585-104">系統管理員可能已停用服務主體，以封鎖 Yammer 的存取權。</span><span class="sxs-lookup"><span data-stu-id="ba585-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="ba585-105">我們不建議您停用服務主體，這可能會導致其他問題。</span><span class="sxs-lookup"><span data-stu-id="ba585-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="ba585-106">如需封鎖使用者存取 Yammer 支援方法的詳細資訊，請參閱 [關閉 Microsoft 365 使用者的 Yammer 存取權](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)。</span><span class="sxs-lookup"><span data-stu-id="ba585-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="ba585-107">以下方法可修正 Azure 入口網站中的這項問題，並還原使用者對 Yammer 的存取權：</span><span class="sxs-lookup"><span data-stu-id="ba585-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="ba585-108">開啟 Azure Active Directory 頁面，然後選取左側瀏覽窗格 **[管理]** 底下的 **[企業應用程式]**。</span><span class="sxs-lookup"><span data-stu-id="ba585-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="ba585-109">在搜尋方塊中輸入 **Office 365 Yammer**，然後選取應用程式名稱以開啟 [設定]。</span><span class="sxs-lookup"><span data-stu-id="ba585-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="ba585-110">選取左側瀏覽窗格 **[管理]** 底下的 **[屬性]**。</span><span class="sxs-lookup"><span data-stu-id="ba585-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="ba585-111">將 **[啟用使用者登入]** 的值設為 **[是]**，然後選取 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="ba585-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="ba585-112">再次登入 Yammer。</span><span class="sxs-lookup"><span data-stu-id="ba585-112">Sign in to Yammer again.</span></span> <span data-ttu-id="ba585-113">您可能需要清除 cookie。</span><span class="sxs-lookup"><span data-stu-id="ba585-113">You might need to clear cookies.</span></span>

<span data-ttu-id="ba585-114">或者，您也可以執行 PowerShell 命令以設定值。</span><span class="sxs-lookup"><span data-stu-id="ba585-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="ba585-115">如需詳細資訊，請參閱 [當您在 Office 365 中點擊 Yammer 磚時，發生錯誤，「很抱歉，您無法登入」](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="ba585-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 