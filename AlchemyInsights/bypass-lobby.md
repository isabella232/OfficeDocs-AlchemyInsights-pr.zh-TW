---
title: 略過大廳
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889073"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="d3758-102">控制大廳設定和參與小組層級</span><span class="sxs-lookup"><span data-stu-id="d3758-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="d3758-103">如果您想要允許所有人，包括撥入式、 外部和匿名使用者，以**略過大廳**，使用 PowerShell 來完成此工作。</span><span class="sxs-lookup"><span data-stu-id="d3758-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="d3758-104">以下是範例修改您組織的全域會議原則。</span><span class="sxs-lookup"><span data-stu-id="d3758-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="d3758-105">此 cmdlet 目前需要使用的 Skype for Business PowerShell 模組。</span><span class="sxs-lookup"><span data-stu-id="d3758-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="d3758-106">若要取得設定為使用此指令程式，請參閱[Managing 透過 PowerShell 的原則](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。</span><span class="sxs-lookup"><span data-stu-id="d3758-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="d3758-107">一旦您已設定的原則，您需要將它套用至使用者。或者，如果您修改全域原則，它會自動將套用至使用者。</span><span class="sxs-lookup"><span data-stu-id="d3758-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="d3758-108">任何原則的變更，您必須至少等待**4 小時設定為 24 小時**才會生效原則。</span><span class="sxs-lookup"><span data-stu-id="d3758-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="d3758-109">請務必檢閱下方之前進行了解完全什麼這可讓這些變更的文件。</span><span class="sxs-lookup"><span data-stu-id="d3758-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="d3758-110">了解 Teams 會議大廳原則控制項</span><span class="sxs-lookup"><span data-stu-id="d3758-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="d3758-111">這些設定會控制其會議參與者等候在大廳之前他們加入會議，參與程度他們允許在會議中。</span><span class="sxs-lookup"><span data-stu-id="d3758-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="d3758-112">您可以使用 PowerShell 來更新會議原則設定尚未尚未實作 （標示為 「 即將推出 」） 中的 Teams 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="d3758-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="d3758-113">請參閱下面範例 PowerShell cmdlet，可讓略過大廳中的所有使用者。</span><span class="sxs-lookup"><span data-stu-id="d3758-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="d3758-114">[自動准許人員](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是控制項是否人員加入會議直接，或在大廳等待，直到他們准許的已驗證使用者的每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="d3758-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="d3758-115">[允許匿名使用者啟動會議](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是控制匿名的人員，包括 B2B 和同盟的使用者，是否可以加入沒有已驗證的使用者從組織的使用者的會議出席者的每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="d3758-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="d3758-116">[允許撥入式使用者略過大廳](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（**即將推出**） 是該控制項的撥號對應表中的人員電話加入會議直接，還是不論**自動准許人員**設定在大廳中等候的每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="d3758-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="d3758-117">[若要覆寫大廳設定允許召集人](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（**即將推出**） 是會議召集人是否可以覆寫為系統管理員設定**自動准許人員**和**允許電話撥入式使用者略過大廳**中，當他們排定新會議大廳設定會控制每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="d3758-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="d3758-118">**附註：** 請閱讀[管理小組中的會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)Microsoft Teams 會議原則的完整概觀。</span><span class="sxs-lookup"><span data-stu-id="d3758-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
