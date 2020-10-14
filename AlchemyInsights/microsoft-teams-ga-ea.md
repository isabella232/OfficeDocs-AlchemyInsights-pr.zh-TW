---
title: Microsoft 團隊-來賓存取
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: ee38dcb5f40ea16cea1b84b9b16e86b0f52f2d89
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/13/2020
ms.locfileid: "48452219"
---
# <a name="microsoft-teams---guest-access"></a><span data-ttu-id="d5546-102">Microsoft 團隊-來賓存取</span><span class="sxs-lookup"><span data-stu-id="d5546-102">Microsoft Teams - Guest Access</span></span>

<span data-ttu-id="d5546-103">如果您需要協助與小組中組織的使用者進行通訊，您必須決定是否要使用 [Guest access 或外部 Access (同盟) ](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)，也可以同時使用這兩者。</span><span class="sxs-lookup"><span data-stu-id="d5546-103">If you need help communicating with users outside your Organization in Teams, you need to decide whether to use [Guest Access or External Access (Federation)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), or you can use both.</span></span>

<span data-ttu-id="d5546-104">請務必 [查看差異](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) ，以瞭解每個可用的功能。</span><span class="sxs-lookup"><span data-stu-id="d5546-104">Be sure to [review the differences](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) to understand the features available for each.</span></span>  <span data-ttu-id="d5546-105">例如，「外部存取 (同盟」) 允許1:1 通訊，例如聊天與顯示狀態。</span><span class="sxs-lookup"><span data-stu-id="d5546-105">For example, External access (federation) allows for 1:1 communications, like Chat and Presence.</span></span>  <span data-ttu-id="d5546-106">不過，同盟使用者無法參與小組共同作業。</span><span class="sxs-lookup"><span data-stu-id="d5546-106">Federated users cannot participate in Teams collaboration however.</span></span>  <span data-ttu-id="d5546-107">如果您想要讓外部使用者加入小組通道交談或共用檔案，您必須開啟來賓存取。</span><span class="sxs-lookup"><span data-stu-id="d5546-107">If you’d like an external user to join and participate in Teams Channel Conversations or Share Files, you’ll need to turn on Guest Access.</span></span>

<span data-ttu-id="d5546-108">**選項1：開啟來賓存取** 在團隊系統管理中心中，移至 [ [Org Wide Settings > Guest access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) ]，然後開啟「允許小組中的來賓存取」。</span><span class="sxs-lookup"><span data-stu-id="d5546-108">**Option 1: Turn on Guest Access** In the Teams Admin Center, Go to [Org Wide Settings > Guest Access](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) and turn on “Allow Guest Access in Teams”.</span></span>  <span data-ttu-id="d5546-109">針對具有所有其他預設設定的承租人，這應該是您需要做的全部工作。</span><span class="sxs-lookup"><span data-stu-id="d5546-109">For a tenant with all other default settings, this should be all you need to do.</span></span>  <span data-ttu-id="d5546-110">若要自訂來賓存取設定，請確定您遵循 [來賓存取檢查清單](https://docs.microsoft.com/microsoftteams/guest-access-checklist)中的所有步驟。</span><span class="sxs-lookup"><span data-stu-id="d5546-110">To customize your Guest Access configuration,  make sure you follow all the steps in the [Guest Access Checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist).</span></span> <span data-ttu-id="d5546-111">完成後，您將需要 [等候24小時](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) ，設定才會生效。</span><span class="sxs-lookup"><span data-stu-id="d5546-111">Once you're completely done, you'll need to [wait up to 24 hours](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) for the settings to take effect.</span></span>

<span data-ttu-id="d5546-112">如果您確信您已完成檢查清單中的所有步驟，且已超過24小時，請繼續進行，並嘗試 [將來賓新增至您的小組](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)。</span><span class="sxs-lookup"><span data-stu-id="d5546-112">If you’re confident you’ve completed all the steps in the Checklist, and it's been more than 24 hours, go ahead and try to [add a Guest to your Team](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).</span></span>

<span data-ttu-id="d5546-113">如需詳細資訊（包括操作方式影片），請參閱 [Microsoft 小組中的 Guest access](https://docs.microsoft.com/microsoftteams/guest-access)。</span><span class="sxs-lookup"><span data-stu-id="d5546-113">For more information, including how-to videos, see [Guest access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).</span></span>

<span data-ttu-id="d5546-114">\*\*選項2：開啟外部存取 (同盟) \*\* 如果您也想要開啟外部存取 (同盟) ，請在團隊系統管理中心移至 [整個組織的設定 > 外部存取](https://admin.teams.microsoft.com/company-wide-settings/external-communications) ，然後開啟「使用者可以與商務用 Skype 和小組使用者通訊」，然後遵循下列所有步驟， [讓您的小組使用者能夠與其他組織中的使用者交談及通訊](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)。</span><span class="sxs-lookup"><span data-stu-id="d5546-114">**Option 2: Turn On External Access (Federation)** If you’d also like to turn on External Access (Federation), in the Teams Admin center go to [Org-wide Settings > External Access](https://admin.teams.microsoft.com/company-wide-settings/external-communications) and turn on "Users can communicate with Skype for Business and Teams users", and then follow all the steps in [Let your Teams users chat and communicate with users in another organization](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).</span></span>
