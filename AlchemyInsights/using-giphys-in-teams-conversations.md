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
# <a name="using-giphys-in-teams-conversations"></a>在小組交談中使用 Giphys

預設會啟用小組聊天的 Giphys 存取。 身為系統管理員，您可以透過 [設定郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)，以控制使用者是否可以使用 Giphys，以及確保已 **開啟** [ **使用 Giphys** ]。

如果 Gif 未如預期的方式在小組交談中運作，請驗證：

[郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)需要允許 Giphys。 若要使用 PowerShell Cmdlet 進行驗證：

- 請確認您可以 [使用 PowerShell 管理團隊](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)。
- 執行 PowerShell 命令 [CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ，並確認 **AllowGiphy** 設定為 **TRUE** 。
- 如果 **AllowGiphy** 設定為 **FALSE** ，請執行下列 PowerShell 命令 [CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)。

若要允許存取 Giphy URL，必須啟用[選用的連線體驗](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)。

> [!NOTE]
> 如果您已針對租使用者設定多個團隊郵件原則，您可以使用 PowerShell 命令，判斷指派給受影響使用者之原則的身分識別 [Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> |選取 [TeamsMessagingPolicy]。
