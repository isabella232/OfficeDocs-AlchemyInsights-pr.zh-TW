---
title: 推遲 Teams 升級
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
- "2737"
- "4000006"
ms.openlocfilehash: 893a01ae74f8aec9bb0079430188e3cd6881b3009818830ea5572cfa41cdf71f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923968"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>如何推遲 Microsoft 導向的 Teams 升級

**重要**：我們可以使用支援診斷來協助您修正此問題，但似乎您並未使用新的系統管理中心。 若要使用新的系統管理中心，請在右上方的 **上方向右** 滑動切換按鈕。 使用新的系統管理中心，按一下 [**需要協助？** ] 小工具，輸入「推遲 Teams 升級」，然後依照提示執行診斷。

如果您收到來自 Microsoft 導向的從商務用 Skype 到 Microsoft Teams 的自動升級的通訊，而您想要將自動升級推遲到日後的日期，您的全域系統管理員可以登入 Teams 的系統 [管理入口網站](https://admin.teams.microsoft.com/dashboard)，然後在 [Microsoft Teams 升級] 下選取 [重新整理 **狀態**] 按鈕後，選取 [**延期**] 按鈕。 若要查看租使用者自動升級至 Microsoft Teams 的新日期，請重新整理 Teams 管理入口網站頁面。

**附注：** [ **延期** ] 按鈕只有在您收到有關自動升級的訊息中心通知時才會使用。 

全域管理員也可以執行 [CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) ，以深入瞭解其目前的升級狀態。
