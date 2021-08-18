---
title: 擷取稽核記錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: ac2e5eafbb92b234697c22f73cd565af9d7c3508
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329485"
---
# <a name="retrieve-the-audit-logs"></a>擷取稽核記錄

首次開啟稽核記錄時，它為空。 請搜尋查看其中有什麼內容。 以下是對所有活動進行一般搜尋的方式：

1. 執行下列其中一個步驟：
   - 在位於 <https://compliance.microsoft.com> 的 Microsoft 365 合規性中心中，前往 **[解決方案]** \> **[稽核]**。 或者，若要直接前往 **[稽核]** 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch>。
   - 在位於 <https://security.microsoft.com> 的 Microsoft 365 Defender 入口網站中，移至 **[稽核]**。 或者，若要直接前往 **[稽核]** 頁面，請使用 <https://sip.security.microsoft.com/auditlogsearch>。

2. 在 **[稽核]** 頁面上，確認已選取 **[搜尋]** 索引標籤，然後設定下列設定：
   - **日期和時間範圍**：在 **[開始]** 和 **[結束]** 方塊中選取日期/時間範圍。
   - **活動**：確認已選取 **[顯示所有活動的結果]**。
   - **使用者**：接受空白預設值以傳回所有使用者的結果，或輸入一或多位使用者。

3. 完成後，按一下 **[搜尋]**。 活動會顯示在新的 **[稽核搜尋]** 頁面上。

4. 在結果中，按一下 **[篩選結果]**，並在活動篩選方塊中輸入 **Set-Mailbox**。

5. 在結果中選取稽核記錄。 在 **[詳細資訊]** 飛出視窗中，按一下 **[詳細資訊]** 以查看更多資訊，如用戶端、執行動作的使用者等。
