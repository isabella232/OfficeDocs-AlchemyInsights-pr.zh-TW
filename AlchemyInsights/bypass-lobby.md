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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>控制大廳設定和參與小組層級

如果您想要允許所有人，包括撥入式、 外部和匿名使用者，以**略過大廳**，使用 PowerShell 來完成此工作。 以下是範例修改您組織的全域會議原則。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

此 cmdlet 目前需要使用的 Skype for Business PowerShell 模組。 若要取得設定為使用此指令程式，請參閱[Managing 透過 PowerShell 的原則](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。

一旦您已設定的原則，您需要將它套用至使用者。或者，如果您修改全域原則，它會自動將套用至使用者。 任何原則的變更，您必須至少等待**4 小時設定為 24 小時**才會生效原則。 

請務必檢閱下方之前進行了解完全什麼這可讓這些變更的文件。


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>了解 Teams 會議大廳原則控制項

這些設定會控制其會議參與者等候在大廳之前他們加入會議，參與程度他們允許在會議中。 您可以使用 PowerShell 來更新會議原則設定尚未尚未實作 （標示為 「 即將推出 」） 中的 Teams 系統管理中心。 請參閱下面範例 PowerShell cmdlet，可讓略過大廳中的所有使用者。

- [自動准許人員](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是控制項是否人員加入會議直接，或在大廳等待，直到他們准許的已驗證使用者的每個組合管理原則。

- [允許匿名使用者啟動會議](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是控制匿名的人員，包括 B2B 和同盟的使用者，是否可以加入沒有已驗證的使用者從組織的使用者的會議出席者的每個組合管理原則。

- [允許撥入式使用者略過大廳](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（**即將推出**） 是該控制項的撥號對應表中的人員電話加入會議直接，還是不論**自動准許人員**設定在大廳中等候的每個組合管理原則。

- [若要覆寫大廳設定允許召集人](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（**即將推出**） 是會議召集人是否可以覆寫為系統管理員設定**自動准許人員**和**允許電話撥入式使用者略過大廳**中，當他們排定新會議大廳設定會控制每個組合管理原則。

**附註：** 請閱讀[管理小組中的會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)Microsoft Teams 會議原則的完整概觀。
