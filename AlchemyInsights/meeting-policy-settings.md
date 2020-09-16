---
title: 會議原則設定
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
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794325"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>在 Microsoft 小組中管理會議原則

**附注：原則變更可能需要24小時才能讓使用者生效。** 您可能無法立即對新建立的原則進行變更。等候4小時，然後嘗試再次修改新建立的原則。

會議原則是用來控制會議參與者對於由組織中的使用者排程的會議參與者可用的功能。 會議原則的某些功能可能無法在團隊系統管理中心中實施，但 (這些功能會在檔) 中標示為「即將推出」。 在此情況下，或是如果您收到錯誤（如「我們無法立即更新原則，但稍後再試一次」）在 Microsoft 團隊系統管理中心，我們建議您使用 PowerShell 建立或修改小組會議原則。 

如需會議原則的詳細資訊，請參閱下列資源：

- 若要瞭解如何建立原則、進行變更，以及將使用者指派給原則，請參閱 [管理小組中的會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。

- 若要使用 PowerShell Cmdlet 進行原則變更，請參閱 [團隊 PowerShell 綜述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。 
    - 您需要針對團隊會議原則使用 [商務用 Skype PowerShell 模組](https://www.microsoft.com/download/details.aspx?id=39366) 。 
    - 如需詳細資訊，請參閱 [*-CsTeamsMeetingPolicy Cmdlet 檔](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 。

