---
title: 尋找對收件匣規則執行的事件
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313490"
---
# <a name="find-events-performed-on-inbox-rules"></a>尋找對收件匣規則執行的事件

建立、變更或刪除收件匣規則時，事件會記錄在審計記錄檔中。 以下說明如何進行檢查：

1. 請執行下列其中一個動作：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

    **附注**：如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。 若未開啟此功能，搜尋結果將無法從先前的日期提取資料。
1. 選取 [活動] 欄位，並尋找 Exchange 信箱活動]，然後從 Outlook Web App 中選取 New-InboxRule 建立收件匣規則。 當您完成時，按一下窗格外以最小化 [活動] 窗格。
1. 指定日期範圍，然後在 [使用者] 欄位中，選取您要調查之使用者的使用者名稱。 您可以一次選取一個以上的使用者。
1. 選取 [搜尋]。 這些活動出現在 [結果] 下。
1. 若要查看詳細資料，請選取活動，然後選取 [詳細資訊]。 在 [參數] 區段中，您可以看到規則的名稱、條件集，以及規則將採取的動作。

2. 在 [**審核**] 頁面的 [**搜尋] 索引** 標籤上，設定下列設定：
   - **日期和時間範圍**：選取 [ **開始** ] 和 [ **結束** ] 方塊中的 [日期/時間範圍]。
   - **活動**：**從 Outlook Web App 選取 [New-InboxRule 建立收件匣規則**]

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 選取結果中的活動，以開啟 [詳細資料] 快顯視窗。 在 [ **參數** ] 區段中，您可以看到規則的名稱、條件集，以及規則將採取的動作。

若要深入瞭解，請參閱 [搜尋審核記錄檔，以調查常見的支援問題](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
