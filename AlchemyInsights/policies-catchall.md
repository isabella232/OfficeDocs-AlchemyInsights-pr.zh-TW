---
title: 原則所限
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "3207"
ms.openlocfilehash: 036c171f3c71e60c8c07000b4d0c6ede36bd435c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801654"
---
# <a name="teams-policies"></a><span data-ttu-id="e2bee-102">小組原則</span><span class="sxs-lookup"><span data-stu-id="e2bee-102">Teams policies</span></span>

<span data-ttu-id="e2bee-103">Microsoft 團隊設定是由原則所控制。</span><span class="sxs-lookup"><span data-stu-id="e2bee-103">Microsoft Teams settings are controlled by policies.</span></span> <span data-ttu-id="e2bee-104">若要進行變更，您必須設定適當的原則，然後將其套用至使用者。</span><span class="sxs-lookup"><span data-stu-id="e2bee-104">To make a change, you must configure the appropriate policy, and then apply it to users.</span></span> <span data-ttu-id="e2bee-105">為所有使用者執行這項作業的最快捷方式是修改名為 Global 的預設原則。</span><span class="sxs-lookup"><span data-stu-id="e2bee-105">The quickest way to do this for all your users is to modify the default policy named Global.</span></span> 

<span data-ttu-id="e2bee-106">**記事** 原則變更 **_至少需要4小時 48 4 小時才會生效_**。</span><span class="sxs-lookup"><span data-stu-id="e2bee-106">**NOTE** Policy changes take **_at least 4 up to 48 hours to take effect_**.</span></span> <span data-ttu-id="e2bee-107">如果您建立自訂原則，至少需要等候4小時，您才能進行其他變更。</span><span class="sxs-lookup"><span data-stu-id="e2bee-107">If you create a custom policy, you need to wait at least 4 hours before you can make additional changes to it.</span></span> <span data-ttu-id="e2bee-108">然後，您就可以將該原則套用至使用者。</span><span class="sxs-lookup"><span data-stu-id="e2bee-108">Then you can apply that policy to users.</span></span> <span data-ttu-id="e2bee-109">這表示自訂原則可能需要長達48小時才會生效。</span><span class="sxs-lookup"><span data-stu-id="e2bee-109">This means that custom policies can take up to 48 hours to take effect.</span></span> <span data-ttu-id="e2bee-110">全域原則會設定為所有使用者的預設值，而且全域原則的變更可能需要長達24小時才會生效。</span><span class="sxs-lookup"><span data-stu-id="e2bee-110">Global policies are set as default for all users, and changes to the Global policy can take up to 24 hours to take effect.</span></span> <span data-ttu-id="e2bee-111">如果您已建立自訂原則，並將其套用至使用者，但在48小時之後仍未生效，或者您已修改全域原則並且等候至少24小時，請開啟支援案例。</span><span class="sxs-lookup"><span data-stu-id="e2bee-111">If you have created a custom policy, applied it to users, and it still hasn't taken effect after 48 hours, or you've modified the Global policy and waited at least 24 hours, please open a support case.</span></span>

<span data-ttu-id="e2bee-112">小組原則分為下列幾個區域：</span><span class="sxs-lookup"><span data-stu-id="e2bee-112">Teams policies are divided into the following areas:</span></span>

- <span data-ttu-id="e2bee-113">[團隊原則](https://docs.microsoft.com/MicrosoftTeams/teams-policies) 會控制使用者在搜尋和建立專用通道的使用者探索。</span><span class="sxs-lookup"><span data-stu-id="e2bee-113">[Teams policies](https://docs.microsoft.com/MicrosoftTeams/teams-policies) control user discovery of private teams in search and creation of private channels.</span></span>  
- <span data-ttu-id="e2bee-114">[會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 控制使用者可以使用團隊會議做什麼，包括控制大廳。</span><span class="sxs-lookup"><span data-stu-id="e2bee-114">[Meeting policies](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) control what users can do with Teams meetings, including controlling the lobby.</span></span> <span data-ttu-id="e2bee-115">如需對會議廳問題的協助，例如設定小組以承認任何人，請參閱 [控制會議廳設定和參與的層級](https://docs.microsoft.com/alchemyinsights/bypass-lobby)。</span><span class="sxs-lookup"><span data-stu-id="e2bee-115">For help with lobby issues, like configuring Teams to admit everyone, see [Control lobby settings and levels of participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby).</span></span>
- <span data-ttu-id="e2bee-116">[郵件原則](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) 控制使用者可以使用聊天和郵件執行的動作，包括開啟或關閉聊天、刪除聊天、要求閱讀回執、使用 giphys 和貼上功能等等。</span><span class="sxs-lookup"><span data-stu-id="e2bee-116">[Messaging policies](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) control what users can do with chat and messages, including turning chat on or off, deleting chats, requesting read receipts, using giphys and stickers, and more.</span></span>
- <span data-ttu-id="e2bee-117">[App 安裝原則](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) 控制使用者可以使用哪些應用程式，包括自訂和協力廠商應用程式，以及顯示的順序。</span><span class="sxs-lookup"><span data-stu-id="e2bee-117">[App setup policies](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) control which apps are available to users, including custom and third-party apps, and the order in which they appear.</span></span>  
- <span data-ttu-id="e2bee-118">小組的資料 [保留原則](https://docs.microsoft.com/microsoftteams/retention-policies) 可在 Microsoft 365 安全性與合規性中心內找到。</span><span class="sxs-lookup"><span data-stu-id="e2bee-118">Data [retention policies](https://docs.microsoft.com/microsoftteams/retention-policies) for Teams are found in the Microsoft 365 security and Compliance Center.</span></span>
- <span data-ttu-id="e2bee-119">小組透過 [範圍的目錄搜尋](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)來設定通訊錄原則。</span><span class="sxs-lookup"><span data-stu-id="e2bee-119">Teams address book policies are set via [scoped directory search](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).</span></span>