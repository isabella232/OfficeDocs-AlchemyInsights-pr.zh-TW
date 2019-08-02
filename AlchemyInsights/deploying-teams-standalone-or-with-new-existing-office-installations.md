---
title: 部署小組，以獨立伺服器或新的或現有的 Office 安裝
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054222"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a><span data-ttu-id="5e660-102">部署小組，以獨立伺服器或新的或現有的 Office 安裝</span><span class="sxs-lookup"><span data-stu-id="5e660-102">Deploying Teams as standalone or with new or existing Office installations</span></span>

<span data-ttu-id="5e660-103">Microsoft Teams 現在是包含過程中的***全新安裝***的 Office 365 專業增強版、 Office 365 商務版和 Office for mac。</span><span class="sxs-lookup"><span data-stu-id="5e660-103">Microsoft Teams is now included as part of ***new installations*** of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span> <span data-ttu-id="5e660-104">如需詳細資訊，請參閱[時將 Microsoft Teams 啟動所隨附的新安裝的 Office？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="5e660-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span></span>

<span data-ttu-id="5e660-105">此外，從開始在每月通道版本 1906年，小組會***新增至現有的安裝***的 Office 365 專業增強版 （和 Office 365 商務版） 更新現有的安裝至最新版本時，執行 Windows 裝置上。</span><span class="sxs-lookup"><span data-stu-id="5e660-105">Additionally, starting with Version 1906 in Monthly Channel, Teams will be ***added to existing installations*** of Office 365 ProPlus (and Office 365 Business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="5e660-106">如需詳細資訊，請參閱[Office 的現有安裝呢？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="5e660-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span></span>

> [!NOTE]
> <span data-ttu-id="5e660-107">如果您不想等待此首度發行排程，您可以將部署小組為獨立為您的使用者藉由[遵循這些指示](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) 或您可以讓使用者自行從安裝 Teams [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)。</span><span class="sxs-lookup"><span data-stu-id="5e660-107">If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) or you can have your users install Teams for themselves from [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span></span>

<span data-ttu-id="5e660-108">如果您的組織尚未準備好部署 microsoft Teams，我們會有您可以從[新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus)的或[現有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)的 Office 安裝排除***Teams***採取的步驟。</span><span class="sxs-lookup"><span data-stu-id="5e660-108">If your organization isn't ready to deploy Teams, we have the steps you can take to ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="5e660-109">如果您想要安裝，但不想小組合作，為使用者自動啟動，它安裝之後，請參閱[防止從自動安裝後啟動的 Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)小組。</span><span class="sxs-lookup"><span data-stu-id="5e660-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="5e660-110">若要***解除安裝 microsoft Teams***從執行 Windows 裝置，請參閱[解除安裝 Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)。</span><span class="sxs-lookup"><span data-stu-id="5e660-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="5e660-111">若要清除 Microsoft Teams 從多部目標電腦或使用者，請參閱[Microsoft Teams 部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。</span><span class="sxs-lookup"><span data-stu-id="5e660-111">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="5e660-112">如果您使用共用的電腦]、 [遠端桌面服務 (RDS) 或 [虛擬桌面基礎結構 (VDI)，請參閱[共用電腦與 VDI 環境與 Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。</span><span class="sxs-lookup"><span data-stu-id="5e660-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span>

<span data-ttu-id="5e660-113">如果您使用 Office for Mac，請參閱[在 Mac 上的 Microsoft Teams 安裝](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。</span><span class="sxs-lookup"><span data-stu-id="5e660-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

> [!NOTE]
> <span data-ttu-id="5e660-114">Teams 安裝之後，它是[自動更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)大約每兩週的新功能和品質更新。</span><span class="sxs-lookup"><span data-stu-id="5e660-114">After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 