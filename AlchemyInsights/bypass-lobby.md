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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654247"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="7dcfe-102">控制項大廳設定和其他參與的層級</span><span class="sxs-lookup"><span data-stu-id="7dcfe-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="7dcfe-103">如果您想要允許所有人，包括撥入式、 外部和匿名使用者略過大廳中，您可以使用 PowerShell，若要這樣做。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="7dcfe-104">以下是範例修改您組織的全域會議原則：</span><span class="sxs-lookup"><span data-stu-id="7dcfe-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7dcfe-105">此 cmdlet 目前需要使用的 Skype for Business PowerShell 模組。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7dcfe-106">若要取得安裝程式以使用此指令程式，請參閱[透過 PowerShell 管理原則](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7dcfe-107">您可以設定新的原則，您必須將它套用至使用者。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="7dcfe-108">如果您修改它將會自動套用至使用者的全域原則。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="7dcfe-109">任何原則的變更，您需要等候至少 4 小時，並設定為 24 小時才會原則生效。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="7dcfe-110">請務必檢閱下方之前進行了解完全什麼這可讓這些變更的文件。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7dcfe-111">了解 Teams 會議大廳原則控制項</span><span class="sxs-lookup"><span data-stu-id="7dcfe-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="7dcfe-112">[自動准許人員](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是控制項是否人員加入會議直接，或在大廳等待，直到他們准許的已驗證使用者的每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7dcfe-113">[允許匿名使用者啟動會議](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是控制匿名的人員，包括 B2B 和同盟的使用者，是否可以加入沒有已驗證的使用者從組織的使用者的會議出席者的每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7dcfe-114">[允許撥入式使用者略過大廳](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（**即將推出**） 是該控制項的撥號對應表中的人員電話加入會議直接，還是不論**自動准許人員**設定在大廳中等候的每個組合管理原則。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7dcfe-115">[若要覆寫大廳設定允許召集人](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（**即將推出**） 是會議召集人是否可以覆寫設定**自動准許人員**和**中的系統管理員允許撥號對應表中的大廳設定會控制每個組合管理原則略過大廳的使用者**當他們排定新會議。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7dcfe-116">**附註：** 請閱讀[管理小組中的會議原則](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)Microsoft Teams 會議原則的完整概觀。</span><span class="sxs-lookup"><span data-stu-id="7dcfe-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
