---
title: 在審計記錄檔中識別收件匣規則活動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383016"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>在審計記錄檔中識別收件匣規則活動

您可以使用安全性 & 合規性中心內的審核記錄搜尋, 來查看收件匣規則事件 (建立、修改及刪除收件匣規則)。

1. 登入[Office 365 安全性 & 規範中心](https://protection.office.com/)

2. 按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。

3. 選取 [**開始日期**] 和 [**結束日期**] 欄位中的日期範圍。

4. 在 [ **Exchange 信箱活動**] 下, 確認 [**活動**] 欄位已設定為 [ **disable-inboxrule 程式建立/修改/啟用/停用收件匣規則**]。

5. Click **Search**.

在結果中, 選取一筆審計記錄。 在 [詳細資料] 快顯視窗中, 按一下 [**詳細資訊**]。 收件匣規則設定的相關資訊會顯示在 [**參數**] 欄位中。

如需詳細資訊, 請參閱[決定使用者建立的收件匣規則](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
