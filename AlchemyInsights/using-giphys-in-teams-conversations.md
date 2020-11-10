---
title: 在小組交談中使用 Giphys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947492"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="77df7-102">在小組交談中使用 Giphys</span><span class="sxs-lookup"><span data-stu-id="77df7-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="77df7-103">預設會啟用小組聊天的 Giphys 存取。</span><span class="sxs-lookup"><span data-stu-id="77df7-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="77df7-104">身為系統管理員，您可以透過 [設定郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)，以控制使用者是否可以使用 Giphys，以及確保已 **開啟** [ **使用 Giphys** ]。</span><span class="sxs-lookup"><span data-stu-id="77df7-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="77df7-105">如果 Gif 未如預期的方式在小組交談中運作，請驗證：</span><span class="sxs-lookup"><span data-stu-id="77df7-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="77df7-106">[郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)需要允許 Giphys。</span><span class="sxs-lookup"><span data-stu-id="77df7-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="77df7-107">若要使用 PowerShell Cmdlet 進行驗證：</span><span class="sxs-lookup"><span data-stu-id="77df7-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="77df7-108">請確認您可以 [使用 PowerShell 管理團隊](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)。</span><span class="sxs-lookup"><span data-stu-id="77df7-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="77df7-109">執行 PowerShell 命令 [CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ，並確認 **AllowGiphy** 設定為 **TRUE** 。</span><span class="sxs-lookup"><span data-stu-id="77df7-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="77df7-110">如果 **AllowGiphy** 設定為 **FALSE** ，請執行下列 PowerShell 命令 [CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)。</span><span class="sxs-lookup"><span data-stu-id="77df7-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="77df7-111">若要允許存取 Giphy URL，必須啟用[選用的連線體驗](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)。</span><span class="sxs-lookup"><span data-stu-id="77df7-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="77df7-112">如果您已針對租使用者設定多個團隊郵件原則，您可以使用 PowerShell 命令，判斷指派給受影響使用者之原則的身分識別 [Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> |選取 [TeamsMessagingPolicy]。</span><span class="sxs-lookup"><span data-stu-id="77df7-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
