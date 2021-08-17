---
title: 在審計記錄檔中識別收件匣規則活動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891286"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>在審計記錄檔中識別收件匣規則活動

您可以使用 Microsoft 365 合規性中心中的「審計記錄搜尋」，以查看收件匣規則事件 (建立、修改及刪除收件匣規則) 。

1. 執行下列其中一個步驟：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

2. 在 [**審核**] 頁面的 [**搜尋] 索引** 標籤上，設定下列設定：
   - **日期和時間範圍**：選取 [ **開始** ] 和 [ **結束** ] 方塊中的 [日期/時間範圍]。
   - **活動**：選取下列一或多個值：
     - **從 Outlook Web App New-InboxRule 建立收件匣規則**
     - **Set-InboxRule 從 Outlook Web App 中修改規則**。
     - **從 Outlook 用戶端更新收件匣規則**

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 選取結果中的活動，以開啟 [詳細資料] 快顯視窗。 [ **參數** ] 欄位中會顯示 [收件匣規則] 設定的相關資訊。

如需詳細資訊，請參閱 [判斷使用者是否建立收件匣規則](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)。
