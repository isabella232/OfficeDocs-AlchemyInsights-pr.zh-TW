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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326788"
---
# <a name="fix-tenant-policy-action-override"></a>修正承租人原則 (動作覆寫) 

其中一個反垃圾郵件原則會影響此郵件。 若要複查原則，請執行下列步驟：

1. 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com/> ，移至 [**電子郵件 &** 共同作業 \> **原則] & 規則** \> 的 [原則] 區段中的 [**威脅原則** \> **反垃圾郵件**]。 

   若要直接移至 [反垃圾郵件原則 **]** 頁面，請使用 <https://security.microsoft.com/antispam>。

2. 在 [ **反垃圾郵件原則** ] 頁面上，按一下原則的名稱 (**類型** 是 **自訂反垃圾郵件原則** 或 **名稱** **Anti-Spam 輸入原則 (預設)**) ，以選取原則。
3. 在出現的 [詳細資料] 快顯視窗中，選取 [**動作**] 區段中的 [**編輯動作**]。
4. 在 [ **郵件動作** ] 區段中，檢查 **垃圾郵件**、 **高可信度垃圾郵件**、 **網路釣魚** 和 **高可信度網路釣魚** 的 verdicts，以查看是否已選取下列任何值：
   - **新增 X 標頭**
   - **將主題行前置文字**
   - **將郵件重新導向至電子郵件地址**
   - **刪除郵件**
   - **無動作**

   套用至所有 Exchange Online Protection 客戶的 **標準設定** 可能會影響郵件。

如需詳細資訊，請參閱[在 EOP 中設定反垃圾郵件原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)。
