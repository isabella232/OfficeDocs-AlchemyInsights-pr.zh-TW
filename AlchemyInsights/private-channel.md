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
# <a name="private-channels-in-microsoft-teams"></a>Microsoft 小組中的專用通道

專用通道是 Microsoft 小組中的新功能。 請注意，無法從標準通道轉換專用通道，反之亦然。

如需私人通道的詳細資訊，例如[專用通道建立和成員資格](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership)和[專用通道 SharePoint 網站](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)的資訊，請參閱[Microsoft 小組中的私人通道](https://docs.microsoft.com/MicrosoftTeams/private-channels)。 

**附注：** 因為尚未支援保留私人通道郵件的設定，所以啟用保留原則的承租人預設不會啟用專用通道。 您可以在團隊系統管理中心啟用專用通道。 此外，請注意，雖然不支援保留私人通道郵件，但支援在專用通道中共用的檔案保留。

**需要新的小組擁有者？**

如果私人管道擁有人離職，您可以透過團隊 Powershell 新增新的小組擁有者。


- 請移至[這裡](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6)安裝團隊 Powershell。

以下是您將需要的 Cmdlet：

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

如需小組 Powershell 的詳細資訊，請參閱[小組 PowerShell 綜述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。
