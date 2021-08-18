---
title: Microsoft Teams 用戶端中未顯示行事曆圖示
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54119995"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Microsoft Teams 用戶端中未顯示行事曆圖示

Teams 中的 [行事 **曆**] 索引標籤需要透過 Exchange Web 服務存取 Exchange 信箱。 Exchange 的信箱可以是線上或 On-Premises。 對於未看到 [行事 **曆**] 索引標籤的線上使用者，請確定他們 [已取得 Exchange Online 信箱的授權，且已啟用信箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。 如果您的使用者已 On-Premises，您必須確認您的混合式設定狀況良好。 使用[混合組態精靈](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) 進行疑難排解。 請注意，[Teams 需要有 Exchange 2016 CU3 或更新版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。

如需詳細資訊及疑難排解步驟，請參閱[疑難排解 Microsoft Teams 和 Exchange Server 互動問題](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)。
