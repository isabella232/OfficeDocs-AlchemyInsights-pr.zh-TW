---
title: 略過大廳
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684941"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>控制團隊中的會議廳設定和參與程度

如果您想要允許所有人（包括撥入、外部和匿名使用者） **略過會議廳**，請使用 PowerShell 來完成這項工作。 以下是修改組織全域會議原則的範例。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

此 Cmdlet 目前需要使用商務用 Skype PowerShell 模組。 若要設定使用此 Cmdlet，請透過 PowerShell 查看 [管理原則](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。

在您設定原則之後，您必須將原則套用至使用者。或者，如果您已修改全域原則，它會自動套用至使用者。 針對任何原則變更，您必須至少等候 **4 小時到24小時** ，原則才會生效。 

請務必先閱讀下列檔，再進行這些變更，以瞭解所允許的功能。


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>瞭解小組會議會議廳原則控制項

這些設定會控制哪些會議參與者會在會議廳中等待，以及在會議中允許他們的參與程度。 您可以使用 PowerShell 來更新小組系統管理中心中「即將 ) 推出」 (標示為「即將推出」的會議原則設定。 如需允許所有使用者略過大廳的 PowerShell Cmdlet 範例，請參閱下一節。

- [[自動承認人員](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)] 是每個召集人原則，可控制人員是否直接加入會議，或在會議廳中等待已驗證使用者的使用者。

- [允許匿名人員開始會議](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) 是一種每個召集人原則，可控制匿名人員（包括 B2B 和同盟使用者）是否可以加入使用者的會議，而不需出席者已驗證的使用者。

- [[允許撥入使用者略過會議廳](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) ** () **是每個召集人原則，以控制撥入的使用者是否直接加入會議，或不論 [**自動承認人員**] 設定，都是在大廳中等候。

- [允許召集人覆寫會議廳設定](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) ** () ** 是每個召集人原則，用來控制會議召集人是否可以覆寫 **系統** 管理員所設定的前廳流覽設定，以及是否 **允許撥入使用者** 在排程新會議時略過會議廳。

**附注：** 如需 Microsoft 團隊會議原則的完整綜述，請參閱 [管理小組中的會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 。
