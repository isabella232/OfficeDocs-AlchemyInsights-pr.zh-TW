---
title: 從 Office 安裝中卸載或排除 Teams
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
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007709"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>從新的或現有的 Office 安裝中卸載或排除 Teams

Microsoft Teams 會包含 Microsoft 365 Apps 企業版、Microsoft 365 Apps 商務版及 Mac 版 Office 的一部分。

- 使用[Office 部署工具](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)，從 Office 的新安裝中排除 Teams。
- 若要從執行 Windows 的裝置 *卸載* Teams，請參閱 [uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)。 若要清理多個目的電腦或使用者的 Microsoft Teams，請參閱[Microsoft Teams 部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。
- 您可以使用[PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
)選項，避免 Microsoft Teams 隨 Office 自動安裝。
- 在 *安裝 Teams 之前*，請使用 [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)選項，以避免 Microsoft Teams 在安裝之後自動啟動。

如果您使用的是 Mac 版 Office，請參閱[Microsoft Teams 安裝上的 Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。