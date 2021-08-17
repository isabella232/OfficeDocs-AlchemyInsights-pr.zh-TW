---
title: 讀取已刪除事件的審計記錄檔
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896006"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>讀取已刪除事件的審計記錄檔

以下說明如何執行此動作：

1. 請執行下列其中一個動作：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

    > [!NOTE]
    > 如果您看到需要開啟此功能的通知，請繼續進行並開啟它。 如果功能未開啟，搜尋結果將無法從先前的日期提取資料。

2. 在 [**審核**] 頁面的 [**搜尋] 索引** 標籤上，設定下列設定：
   - **日期和時間範圍**：選取 [ **開始** ] 和 [ **結束** ] 方塊中的 [日期/時間範圍]。
   - **活動**：輸入 **Exchange 信箱活動**，然後選取下列值：
     - **已刪除 [刪除的郵件] 資料夾中的郵件**
     - **已移動郵件至 [刪除的郵件] 資料夾**

       當您完成時，按一下窗格外以最小化 [ **活動** ] 窗格。

   - **使用者**：接受空白預設值以傳回所有使用者的結果，或輸入一或多個使用者。

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 選取結果中的活動，以開啟 [詳細資料] 快顯視窗。 在 [ **AffectedItems** ] 欄位中會顯示刪除專案的其他資訊，例如專案的主旨行和位置。

   > [!NOTE]
   > 您無法使用「審核記錄」功能還原已刪除的專案。 若要還原刪除的專案，請參閱[在 Outlook 網頁版中復原已刪除的電子郵件](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)。

如需詳細資訊，請參閱 [搜尋審核記錄檔以調查常見的支援問題](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
