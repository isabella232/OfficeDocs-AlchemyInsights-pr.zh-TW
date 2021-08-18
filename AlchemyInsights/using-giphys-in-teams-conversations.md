---
title: 在 Teams 交談中使用 Giphys
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323511"
---
# <a name="using-giphys-in-teams-conversations"></a>在 Teams 交談中使用 Giphys

預設會啟用 Teams 聊天中的 Giphys 存取。 身為系統管理員，您可以透過 [設定郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)，以控制使用者是否可以使用 Giphys，以及確保已 **開啟**[**使用 Giphys** ]。

如果 gif Teams 交談中未如預期的方式運作，請驗證：

[郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)需要允許 Giphys。 若要使用 PowerShell Cmdlet 進行驗證：

- 請確認您可以[使用 PowerShell 管理 Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)。
- 執行 PowerShell 命令 [CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ，並確認 **AllowGiphy** 設定為 **TRUE**。
- 如果 **AllowGiphy** 設定為 **FALSE**，請執行下列 PowerShell 命令 [CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)。

若要允許存取 Giphy URL，必須啟用[選用的連線體驗](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)。

**附注**：如果您已針對租使用者設定多個 Teams 郵件原則，您可以使用 PowerShell 命令，判斷指派給受影響使用者之原則的身分識別 [Get-CsOnlineUser 身分識別](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> |選取 [TeamsMessagingPolicy]。
