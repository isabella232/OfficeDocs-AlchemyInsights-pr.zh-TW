---
title: 封鎖使用者記錄會議
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019175"
---
# <a name="block-user-from-recording-meetings"></a>封鎖使用者記錄會議

如果您需要 **防止或封鎖** 特定使用者錄製 Teams 會議，您可以透過 Teams 會議原則設定來執行。 在 Microsoft Teams 系統管理中心，關閉指派給該使用者的會議原則中的 [**允許雲端錄製**] 設定。 若要深入瞭解，請參閱[Manage meeting 原則 in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)。

若要驗證是否允許某特定使用者或不錄製 Teams 會議，請使用支援診斷。 執行新的支援查詢並輸入 **診斷：會議錄製** -診斷會檢查指定使用者的原則設定，並決定其原則設定。 請記住，新原則設定會有幾個小時的時間生效，所以如果您剛進行變更，請稍候幾小時，再重新執行診斷。

如需詳細資訊，請參閱 [開啟或關閉雲端錄製](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)。
