---
title: 擷取稽核記錄
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320434"
---
# <a name="retrieve-the-audit-logs"></a>擷取稽核記錄

當您第一次開啟審計記錄檔時，它會是空的。 請搜尋查看其中有什麼內容。 以下是對所有活動進行一般搜尋的方式：

1. 請執行下列其中一個動作：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

2. 在 [**審核**] 頁面的 [**搜尋] 索引** 標籤上，設定下列設定：
   - **日期和時間範圍**：選取 [ **開始** ] 和 [ **結束** ] 方塊中的 [日期/時間範圍]。
   - **活動**： Verify 會選取 [ **顯示所有活動的結果** ]。
   - **使用者**：接受空白預設值以傳回所有使用者的結果，或輸入一或多個使用者。

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 選取結果中的活動，以開啟 [詳細資料] 快顯視窗。 您將會看到其他資訊，例如用戶端、執行動作的使用者等等。

若要深入瞭解，請參閱 [搜尋審核記錄檔，以調查常見的支援問題](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
