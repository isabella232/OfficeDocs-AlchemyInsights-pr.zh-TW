---
title: 將小組部署為獨立或現有或現有的 Office 安裝
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 4b843407f05db207f3b676c03c7088d3d0ba062e
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704624"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>將小組部署為獨立或現有或現有的 Office 安裝

Microsoft 團隊現在已包含 Microsoft 365 應用程式的***新安裝***、商務用 Microsoft 365 應用程式和 Mac 版 Office 的一部分。 如需詳細資訊，請參閱[Office 的新安裝會何時開始使用 Microsoft 團隊？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

此外，從每月通道的版本1906開始，當您將現有的安裝更新為最新版本時，小組會新增至執行 Windows 之裝置的現有 Microsoft 365 應用程式（和 Microsoft 365 應用程式）的***現有安裝***。 如需詳細資訊，請參閱[Office 現有安裝的相關資訊？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> 如果您不想要等待此首展排程，您可以[遵循這些指示](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ，將團隊部署為獨立的使用者，也可以讓您的使用者自行安裝團隊 [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)。

[！附注] 如果您的組織未準備好部署小組，我們可以採取步驟來從 Office 的[新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)安裝或[現有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)安裝中***排除團隊***。 如果您想要安裝團隊，但不想讓小組在安裝之後自動為使用者啟動，請參閱在[安裝後自動啟動 [阻止 Microsoft 小組](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)]。

若要從執行 Windows 的裝置***卸載小組***，請參閱[卸載 Microsoft 團隊](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)。 若要從多個目的電腦或使用者清理 Microsoft 團隊，請參閱[Microsoft 團隊部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。

如果您使用的是共用電腦、遠端桌面服務（RDS）或虛擬桌面基礎結構（VDI），請參閱[共用電腦和 VDI 環境與 Microsoft 團隊](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。

如果您使用的是 Mac 版 Office，請參閱[mac 上的 Microsoft 團隊安裝](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。

> [!NOTE]
> 小組安裝完畢後，每兩周[都會自動更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)一次，並提供新功能和品質更新。 