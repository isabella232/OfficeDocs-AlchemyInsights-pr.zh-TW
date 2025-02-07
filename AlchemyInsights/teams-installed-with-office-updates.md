---
title: 隨 Office 更新一起安裝的 Teams
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: c473a001d1441362baad9feb44323b46f1cef42d3c431ef87f0fb0172f10d152
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048723"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>隨 Office 更新一起安裝的 Microsoft Teams

Microsoft Teams 會包含在 ***新安裝*** 的 Microsoft 365 Apps 企業版、Microsoft 365 Apps 商務版及 Mac 版 Office 中。 如需詳細資訊，請參閱[何時 Microsoft Teams 會在新安裝的 Office 中包含 [開始](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)時間]？

此外，在目前通道中從版本1906開始，當您將現有的安裝更新為最新版本時，Teams 會逐漸新增至執行) 之裝置上 Microsoft 365 Apps 企業版 (和 Microsoft 365 Apps 商務版 Windows 的 ***現有安裝***。 如需詳細資訊，請參閱[Office 現有安裝的相關專案？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**附注：** 如果您不想要等待此首展排程，您可以 [遵循下列指示](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)，將 Teams 為您的使用者部署，也可以讓您的使用者自行安裝 Teams https://teams.microsoft.com/downloads 。

如果您的組織未準備好部署 Teams，您可以從 Office 的 [新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)安裝或 [現有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)安裝中 ***排除 Teams*** 。 如果您想要安裝 Teams，但不想讓使用者在安裝之後自動啟動 Teams，請參閱[禁止 Microsoft Teams 在安裝之後自動](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)啟動。

若要從執行 Windows 的裝置 ***卸載 Teams*** ，請參閱 [uninstall Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81)。 若要清理多個目的電腦或使用者的 Microsoft Teams，請參閱[Microsoft Teams 部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。

如果您使用的是共用電腦，則遠端桌面服務 (RDS) 或虛擬桌面基礎結構 (VDI) ，請參閱[共用電腦及 VDI 環境與 Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。 如果您使用的是 Mac 版 Office，請參閱[Microsoft Teams 安裝上的 Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。

**附注：** 安裝 Teams 之後，它會每兩周 [會自動更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)一次，並提供新功能和品質更新。 