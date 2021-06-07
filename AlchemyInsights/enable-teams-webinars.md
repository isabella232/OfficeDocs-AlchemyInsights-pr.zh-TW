---
title: 啟用 Teams 網路研討會
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760836"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="bd8c9-102">啟用 Teams 網路研討會</span><span class="sxs-lookup"><span data-stu-id="bd8c9-102">Enable Teams Webinars</span></span>

<span data-ttu-id="bd8c9-103">預設啟用網路研討會。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-103">Webinars are enabled by default.</span></span> <span data-ttu-id="bd8c9-104">您可以透過使用 Teams PowerShell 命令管理可以排程和註冊 Teams 網路研討會的人員。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="bd8c9-105">所有可以建立會議的使用者也可以建立網路研討會會議。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="bd8c9-106">如果您想要管理可以排程 Teams 網路研討會的人員，請使用 *AllowMeetingRegistration*。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="bd8c9-107">根據預設，*WhoCanRegister* 為啟用狀態且設為 **所有人**。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="bd8c9-108">如果您想要關閉會議註冊，請將 *AllowMeetingRegistration* 設為 **FALSE**。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="bd8c9-109">若要變更這些設定，您必須安裝 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="bd8c9-110">同時，會議原則會在 Teams 網路研討會上強制執行。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="bd8c9-111">舉例來說，如果在會議設定將匿名參加設為關閉，匿名使用者就無法參加網路研討會。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="bd8c9-112">若要深入了解設定可以註冊網路研討會的人員，請參閱 [設定可以註冊網路研討會的人員](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="bd8c9-113">如需 Microsoft 清單設定的詳細資料，請參閱 [控制 Microsoft 清單設定](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="bd8c9-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>