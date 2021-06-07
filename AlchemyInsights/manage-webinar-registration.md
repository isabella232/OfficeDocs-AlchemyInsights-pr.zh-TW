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
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783138"
---
# <a name="manage-webinar-registration"></a>管理網路研討會登錄

您可以透過使用 Teams Powershell 命令來管理可以註冊 Teams 網路研討會的人員。 若要安裝 Teams Powershell，請參閱 [Teams PowerShell](/microsoftteams/teams-powershell-install)。 

根據預設，*WhoCanRegister* 為啟用且設為 **EveryoneInCompany**。 若要允許任何人註冊 (包括匿名使用者)，您必須使用 Powershell 命令將會議原則設定為 [所有人]：

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**附註**：如果在會議設定將 [匿名加入] 設為關閉，匿名使用者就無法加入網路研討會。 若要深入了解並啟用此設定，請參閱[在 Microsoft Teams 中管理會議設定](/microsoftteams/meeting-settings-in-teams)。

如果您想要關閉會議註冊，請將 *AllowMeetingRegistration* 設為 **False**。

若要深入了解設定可以註冊網路研討會的人員，請參閱 [設定可以註冊網路研討會的人員](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。 如需 Microsoft 清單設定的詳細資料，請參閱 [控制 Microsoft 清單設定](/sharepoint/control-lists)。
