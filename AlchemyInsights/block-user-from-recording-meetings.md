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
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897673"
---
# <a name="block-user-from-recording-meetings"></a>封鎖使用者記錄會議

如果您需要 **防止或封鎖** 特定使用者的錄製小組會議，您可以透過團隊會議原則設定來執行此動作。 在 Microsoft 團隊系統管理中心，關閉指派給該使用者的會議原則中的 [ **允許雲端錄製** ] 設定。 若要深入瞭解，請參閱 [管理小組中的會議原則](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)。

若要驗證是否允許特定使用者或不記錄小組會議，請使用支援診斷。 執行新的支援查詢並輸入 **診斷：會議錄製** -診斷會檢查指定使用者的原則設定，並決定其原則設定。 請記住，新原則設定會有幾個小時的時間生效，所以如果您剛進行變更，請稍候幾小時，再重新執行診斷。

如需詳細資訊，請參閱 [開啟或關閉雲端錄製](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)。
