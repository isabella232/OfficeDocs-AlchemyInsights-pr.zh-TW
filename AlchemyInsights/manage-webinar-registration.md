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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760824"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="1d888-102">管理網路研討會登錄</span><span class="sxs-lookup"><span data-stu-id="1d888-102">Manage webinar registration</span></span>

<span data-ttu-id="1d888-103">您可以透過使用 Teams PowerShell 命令管理可以註冊 Teams 網路研討會的人員。</span><span class="sxs-lookup"><span data-stu-id="1d888-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="1d888-104">根據預設，*WhoCanRegister* 為啟用狀態且設為 **所有人**。</span><span class="sxs-lookup"><span data-stu-id="1d888-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="1d888-105">如果您想要關閉會議註冊，請將 *AllowMeetingRegistration* 設為 **FALSE**。</span><span class="sxs-lookup"><span data-stu-id="1d888-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="1d888-106">若要變更這些設定，您必須安裝 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="1d888-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="1d888-107">同時，會議原則會在 Teams 網路研討會上強制執行。</span><span class="sxs-lookup"><span data-stu-id="1d888-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="1d888-108">舉例來說，如果在會議設定將匿名參加設為關閉，匿名使用者就無法參加網路研討會。</span><span class="sxs-lookup"><span data-stu-id="1d888-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="1d888-109">若要深入了解設定可以註冊網路研討會的人員，請參閱 [設定可以註冊網路研討會的人員](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="1d888-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="1d888-110">如需 Microsoft 清單設定的詳細資料，請參閱 [控制 Microsoft 清單設定](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="1d888-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>