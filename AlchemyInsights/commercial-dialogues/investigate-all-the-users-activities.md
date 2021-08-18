---
title: 調查所有使用者的活動
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332334"
---
# <a name="investigate-all-the-users-activities"></a>調查所有使用者的活動

以下說明如何執行此動作：

1. 請執行下列其中一個動作：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

    **附注**：如果您看到需要開啟此功能的通知，請繼續操作，然後立即開啟。 如果功能未開啟，搜尋結果將無法從先前的日期提取資料。

2. 在 [**審核**] 頁面的 [**搜尋] 索引** 標籤上，設定下列設定：
   - **日期和時間範圍**：選取 [ **開始** ] 和 [ **結束** ] 方塊中的 [日期/時間範圍]。
   - **活動**：如果您對特定的活動感興趣，請從清單中進行選取，然後按一下 [是]。否則，預設值會 **顯示所有活動的結果** 會傳回所有活動。
   - **使用者**：接受空白預設值以傳回所有使用者的結果，或輸入一或多個使用者。

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。 您會看到 **IP 位址**、 **使用者** 及 **活動** 名稱。

4. 若要下載結果，請選取 [ **匯出**] [ \> **下載所有結果**]。

5. 選取結果中的活動，以開啟 [詳細資料] 快顯視窗。

若要深入瞭解，請參閱 [搜尋審核記錄檔，以調查常見的支援問題](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
