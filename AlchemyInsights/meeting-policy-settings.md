---
title: 會議原則設定
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
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925156"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>在 Microsoft Teams 中管理會議原則

**附注：原則變更可能需要24小時才能讓使用者生效。** 您可能無法立即對新建立的原則進行變更。等候4小時，然後嘗試再次修改新建立的原則。

會議原則是針對由您組織中的使用者所排程的會議，控制會議參與者可用於會議的功能。 會議原則的某些功能可能無法在 Teams 系統管理中心中實施，但 (這些功能會在檔) 中標示為「即將推出」。 在此情況下，或者如果您收到的錯誤類似 "我們無法立即更新原則，但稍後再試一次，請在 Microsoft Teams 系統管理中心] 中，建議您使用 PowerShell 建立或修改 Teams 會議原則。 

如需會議原則的詳細資訊，請參閱下列資源：

- 若要瞭解如何建立原則、進行變更，以及將使用者指派給原則，請參閱[在 Teams 中管理會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。

- 若要使用 PowerShell Cmdlet 進行原則變更，請參閱[Teams PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。 
    - 您必須使用[商務用 Skype PowerShell 模組](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector)才能 Teams 會議原則。 
    - 如需詳細資訊，請參閱 [*-CsTeamsMeetingPolicy Cmdlet 檔](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 。

