---
title: 推遲小組升級
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801222"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="147e8-102">如何推遲 Microsoft 導向的小組升級</span><span class="sxs-lookup"><span data-stu-id="147e8-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="147e8-103">**重要**：我們可以使用支援診斷來協助您修正此問題，但似乎您並未使用新的系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="147e8-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="147e8-104">若要使用新的系統管理中心，請在右上方的 **上方向右** 滑動切換按鈕。</span><span class="sxs-lookup"><span data-stu-id="147e8-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="147e8-105">使用新的系統管理中心，按一下 [ **需要協助？** ] 小工具，輸入「推遲小組升級」，然後遵循提示執行診斷。</span><span class="sxs-lookup"><span data-stu-id="147e8-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="147e8-106">如果您收到從商務用 Skype 到 Microsoft 小組之 Microsoft 導向的自動升級的通訊，而您想要將自動升級推遲到日後的日期，您的全域系統管理員可以登入 [小組管理員入口網站](https://admin.teams.microsoft.com/dashboard) ，然後在 [Microsoft 團隊升級] 下選取 [重新整理 **狀態** ] 按鈕之後，選取 [ **延遲** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="147e8-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="147e8-107">若要查看租使用者自動升級至 Microsoft 小組的新日期，請重新整理「小組管理入口網站」頁面。</span><span class="sxs-lookup"><span data-stu-id="147e8-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="147e8-108">**附注：** [ **延期** ] 按鈕只有在您收到有關自動升級的訊息中心通知時才會使用。</span><span class="sxs-lookup"><span data-stu-id="147e8-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="147e8-109">全域管理員也可以執行 [CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) ，以深入瞭解其目前的升級狀態。</span><span class="sxs-lookup"><span data-stu-id="147e8-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
