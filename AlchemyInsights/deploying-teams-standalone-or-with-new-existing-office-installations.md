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
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a><span data-ttu-id="72795-102">將小組部署為獨立或現有或現有的 Office 安裝</span><span class="sxs-lookup"><span data-stu-id="72795-102">Deploying Teams as standalone or with new or existing Office installations</span></span>

<span data-ttu-id="72795-103">Microsoft 團隊現在已包含 Microsoft 365 應用程式的***新安裝***、商務用 Microsoft 365 應用程式和 Mac 版 Office 的一部分。</span><span class="sxs-lookup"><span data-stu-id="72795-103">Microsoft Teams is now included as part of ***new installations*** of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span> <span data-ttu-id="72795-104">如需詳細資訊，請參閱[Office 的新安裝會何時開始使用 Microsoft 團隊？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="72795-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span></span>

<span data-ttu-id="72795-105">此外，從每月通道的版本1906開始，當您將現有的安裝更新為最新版本時，小組會新增至執行 Windows 之裝置的現有 Microsoft 365 應用程式（和 Microsoft 365 應用程式）的***現有安裝***。</span><span class="sxs-lookup"><span data-stu-id="72795-105">Additionally, starting with Version 1906 in Monthly Channel, Teams will be ***added to existing installations*** of Microsoft 365 Apps for enterprise (and Microsoft 365 Apps for business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="72795-106">如需詳細資訊，請參閱[Office 現有安裝的相關資訊？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="72795-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span></span>

> [!NOTE]
> <span data-ttu-id="72795-107">如果您不想要等待此首展排程，您可以[遵循這些指示](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) ，將團隊部署為獨立的使用者，也可以讓您的使用者自行安裝團隊 [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)。</span><span class="sxs-lookup"><span data-stu-id="72795-107">If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) or you can have your users install Teams for themselves from [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span></span>

<span data-ttu-id="72795-108">[！附注] 如果您的組織未準備好部署小組，我們可以採取步驟來從 Office 的[新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)安裝或[現有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)安裝中***排除團隊***。</span><span class="sxs-lookup"><span data-stu-id="72795-108">If your organization isn't ready to deploy Teams, we have the steps you can take to ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="72795-109">如果您想要安裝團隊，但不想讓小組在安裝之後自動為使用者啟動，請參閱在[安裝後自動啟動 [阻止 Microsoft 小組](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)]。</span><span class="sxs-lookup"><span data-stu-id="72795-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="72795-110">若要從執行 Windows 的裝置***卸載小組***，請參閱[卸載 Microsoft 團隊](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)。</span><span class="sxs-lookup"><span data-stu-id="72795-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="72795-111">若要從多個目的電腦或使用者清理 Microsoft 團隊，請參閱[Microsoft 團隊部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。</span><span class="sxs-lookup"><span data-stu-id="72795-111">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="72795-112">如果您使用的是共用電腦、遠端桌面服務（RDS）或虛擬桌面基礎結構（VDI），請參閱[共用電腦和 VDI 環境與 Microsoft 團隊](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。</span><span class="sxs-lookup"><span data-stu-id="72795-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span>

<span data-ttu-id="72795-113">如果您使用的是 Mac 版 Office，請參閱[mac 上的 Microsoft 團隊安裝](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。</span><span class="sxs-lookup"><span data-stu-id="72795-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

> [!NOTE]
> <span data-ttu-id="72795-114">小組安裝完畢後，每兩周[都會自動更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)一次，並提供新功能和品質更新。</span><span class="sxs-lookup"><span data-stu-id="72795-114">After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 