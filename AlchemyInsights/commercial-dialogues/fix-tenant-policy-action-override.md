---
title: '修正承租人原則 (動作覆寫) '
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735975"
---
# <a name="fix-tenant-policy-action-override"></a>修正承租人原則 (動作覆寫) 

您租使用者中的反垃圾郵件原則會影響此郵件。 若要查看原則，請執行下列操作：

1. 移至 [Office 365 Security & 合規性中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)，然後移至 **威脅管理**  >  **原則**  >  [反垃圾郵件](https://go.microsoft.com/fwlink/?linkid=2101518)。
2. 查看 [ **原則來源** ] 是否指出下列專案：  **載入 Xheader/ModifySubject/重新導向/刪除/否動作/BCC 郵件**

    如果是的話，在 [ **自訂** ] 索引標籤上，檢查會影響郵件之原則的設定。 適用于所有 Exchange Online Protection 客戶的 **標準設定** 可能會影響郵件。

如需設定垃圾郵件篩選原則的詳細資訊，請參閱 [設定垃圾郵件篩選原則](https://go.microsoft.com/fwlink/?linkid=2101431)。
