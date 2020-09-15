---
title: 使用 Office 更新安裝的小組
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9a09800fcc36876629c7d59182f20b5b16393ef8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47736495"
---
# <a name="microsoft-teams-installed-with-office-updates"></a><span data-ttu-id="4e7b6-102">使用 Office 更新安裝的 Microsoft 團隊</span><span class="sxs-lookup"><span data-stu-id="4e7b6-102">Microsoft Teams installed with Office updates</span></span>

<span data-ttu-id="4e7b6-103">Microsoft 團隊會包含在 ***新安裝*** 的 Microsoft 365 應用程式、商務用 Microsoft 365 應用程式和 Mac 版 Office 的一部分中。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-103">Microsoft Teams is included as part of ***new installations*** of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span> <span data-ttu-id="4e7b6-104">如需詳細資訊，請參閱 [Office 的新安裝會何時開始使用 Microsoft 團隊？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="4e7b6-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="4e7b6-105">此外，從目前通道的版本1906開始，小組會逐漸新增至 ***現有*** 的 Microsoft 365 apps for enterprise (和 Microsoft 365 apps for business) 在將現有安裝更新為最新版本時執行 Windows 的裝置上。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-105">Additionally, starting with Version 1906 in Current Channel , Teams will gradually be added to ***existing installations*** of Microsoft 365 Apps for enterprise (and Microsoft 365 Apps for business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="4e7b6-106">如需詳細資訊，請參閱 [Office 現有安裝的相關資訊？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="4e7b6-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="4e7b6-107">**附注：** 如果您不想要等待此首展排程，您可以 [遵循這些指示](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)，將團隊部署為獨立的使用者，也可以讓您的使用者自行安裝團隊 https://teams.microsoft.com/downloads 。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-107">**Note:** If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment), or you can have your users install Teams for themselves from https://teams.microsoft.com/downloads.</span></span>

<span data-ttu-id="4e7b6-108">如果您的組織未準備好部署小組，您可以從 Office 的[新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)安裝或[現有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)安裝中***排除團隊***。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-108">If your organization isn't ready to deploy Teams, you can ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="4e7b6-109">如果您想要安裝團隊，但不想讓小組在安裝之後自動為使用者啟動，請參閱在 [安裝後自動啟動 [阻止 Microsoft 小組](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)]。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="4e7b6-110">若要從執行 Windows 的裝置 ***卸載小組*** ，請參閱 [卸載 Microsoft 團隊](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81)。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="4e7b6-111">若要從多個目的電腦或使用者清理 Microsoft 團隊，請參閱 [Microsoft 團隊部署清除](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-111">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment cleanup](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="4e7b6-112">如果您使用的是共用電腦，則遠端桌面服務 (RDS) 或虛擬桌面基礎結構 (VDI) ，請參閱 [共用電腦和 VDI 環境與 Microsoft 團隊](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span> <span data-ttu-id="4e7b6-113">如果您使用的是 Mac 版 Office，請參閱 [mac 上的 Microsoft 團隊安裝](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

<span data-ttu-id="4e7b6-114">**附注：** 小組安裝完畢後，每兩周 [都會自動更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 一次，並提供新功能和品質更新。</span><span class="sxs-lookup"><span data-stu-id="4e7b6-114">**Note:** After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 