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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779042"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>在審計記錄檔中識別收件匣規則活動

您可以在 Microsoft 365 Security & 合規性中心內使用審核記錄搜尋，以查看收件匣規則事件 (建立、修改及刪除收件匣規則) 。

1. 登入 [Microsoft 365 的安全性 & 規範中心](https://protection.office.com/)。

2. 移至 [**搜尋**  >  **審核記錄搜尋**] 頁面。

3. 在 [ **開始日期** ] 和 [ **結束日期** ] 欄位中，選取日期範圍。

4. 在 [ **Exchange 信箱活動**] 底下，確認 [ **活動** ] 欄位已設定為 **New-InboxRule 建立/修改/啟用/停用收件匣規則**。

5. 按一下 [搜尋]。

在結果中，選取一個審計記錄。 在 [詳細資料] 快顯視窗中，按一下 [ **詳細資訊**]。 [ **參數** ] 欄位中會顯示 [收件匣規則] 設定的相關資訊。

如需詳細資訊，請參閱 [判斷使用者是否建立收件匣規則](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
