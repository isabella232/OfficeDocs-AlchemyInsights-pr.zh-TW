---
title: 專用通道
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005429"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="19af1-102">Microsoft 小組中的專用通道</span><span class="sxs-lookup"><span data-stu-id="19af1-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="19af1-103">專用通道是 Microsoft 小組中的新功能。</span><span class="sxs-lookup"><span data-stu-id="19af1-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="19af1-104">請注意，無法從標準通道轉換專用通道，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="19af1-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="19af1-105">如需私人通道的詳細資訊，例如[專用通道建立和成員資格](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)和[專用通道 SharePoint 網站](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)的資訊，請參閱[Microsoft 小組中的私人通道](https://docs.microsoft.com/MicrosoftTeams/private-channels)。</span><span class="sxs-lookup"><span data-stu-id="19af1-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="19af1-106">**附注：** 因為尚未支援保留私人通道郵件的設定，所以啟用保留原則的承租人預設不會啟用專用通道。</span><span class="sxs-lookup"><span data-stu-id="19af1-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="19af1-107">您可以在團隊系統管理中心啟用專用通道。</span><span class="sxs-lookup"><span data-stu-id="19af1-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="19af1-108">此外，請注意，雖然不支援保留私人通道郵件，但支援在專用通道中共用的檔案保留。</span><span class="sxs-lookup"><span data-stu-id="19af1-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="19af1-109">**需要新的小組擁有者？**</span><span class="sxs-lookup"><span data-stu-id="19af1-109">**Need a new team owner?**</span></span>

<span data-ttu-id="19af1-110">如果私人管道擁有人離職，您可以透過團隊 Powershell 新增新的小組擁有者。</span><span class="sxs-lookup"><span data-stu-id="19af1-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="19af1-111">請移至[這裡](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)安裝團隊 Powershell。</span><span class="sxs-lookup"><span data-stu-id="19af1-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="19af1-112">以下是您將需要的 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="19af1-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="19af1-113">如需小組 Powershell 的詳細資訊，請參閱[小組 PowerShell 綜述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。</span><span class="sxs-lookup"><span data-stu-id="19af1-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
