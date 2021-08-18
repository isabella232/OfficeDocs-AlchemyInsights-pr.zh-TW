---
title: 修正語言/IP 篩選原則
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
ms.openlocfilehash: 25744bee6f3ed06ae67fc3c246c7d64fce9994bb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320516"
---
# <a name="fix-languageip-filter-policy"></a>修正語言/IP 篩選原則

其中一個反垃圾郵件原則會影響此郵件。 若要複查原則，請執行下列步驟：

1. 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com/> ，移至 [**電子郵件 &** 共同作業 \> **原則] & 規則** \> 的 [原則] 區段中的 [**威脅原則** \> **反垃圾郵件**]。 

   若要直接移至 [反垃圾郵件原則 **]** 頁面，請使用 <https://security.microsoft.com/antispam>。

2. 在 [ **反垃圾郵件原則** ] 頁面上，按一下原則的名稱 (**類型** 是 **自訂反垃圾郵件原則** 或 **名稱** **Anti-Spam 輸入原則 (預設)**) ，以選取原則。
3. 在出現的 [詳細資料] 浮出視窗中，選取 [在 **大量電子郵件閥值 & 垃圾郵件屬性**] 區段中的 [**編輯垃圾郵件閾值**
4. 在 [ **標記為垃圾郵件** ] 區段中，複查 [ **包含特定語言** 和 **這些國家/地區** ] 設定。

如需詳細資訊，請參閱[在 EOP 中設定反垃圾郵件原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)。
