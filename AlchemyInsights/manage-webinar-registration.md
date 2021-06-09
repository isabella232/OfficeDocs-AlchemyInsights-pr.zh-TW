---
title: 管理網路研討會登錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798635"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="01459-102">管理網路研討會登錄</span><span class="sxs-lookup"><span data-stu-id="01459-102">Manage webinar registration</span></span>

<span data-ttu-id="01459-103">您可以透過使用 Teams Powershell 命令來管理可以註冊 Teams 網路研討會的人員。</span><span class="sxs-lookup"><span data-stu-id="01459-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="01459-104">若要安裝 Teams Powershell，請參閱 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="01459-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="01459-105">根據預設，*WhoCanRegister* 為啟用狀態且設為 **所有人**。</span><span class="sxs-lookup"><span data-stu-id="01459-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="01459-106">如果您沒有在會議邀請中看到允許所有人的註冊，請重新執行設定 *WhoCanRegister* 為所有人，並等候 24 小時。</span><span class="sxs-lookup"><span data-stu-id="01459-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="01459-107">若要重新執行 *WhoCanRegister*，請使用 PowerShell 命令：</span><span class="sxs-lookup"><span data-stu-id="01459-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="01459-108">**附註**：如果在會議設定將 [匿名加入] 設為關閉，匿名使用者就無法加入網路研討會。</span><span class="sxs-lookup"><span data-stu-id="01459-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="01459-109">若要深入了解並啟用此設定，請參閱[在 Microsoft Teams 中管理會議設定](/microsoftteams/meeting-settings-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="01459-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="01459-110">如果您想要關閉會議註冊，請將 *AllowMeetingRegistration* 設為 **False**。</span><span class="sxs-lookup"><span data-stu-id="01459-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="01459-111">若要深入了解設定可以註冊網路研討會的人員，請參閱 [設定可以註冊網路研討會的人員](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="01459-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="01459-112">如需 Microsoft 清單設定的詳細資料，請參閱 [控制 Microsoft 清單設定](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="01459-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
