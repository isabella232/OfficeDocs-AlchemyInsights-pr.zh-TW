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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630168"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>在審計記錄檔中識別收件匣規則活動

您可以在「Microsoft 365 安全性 & 相容性中心」中使用審核記錄搜尋，以查看收件匣規則事件 (建立、修改及刪除收件匣規則) 。

1. 登入[Microsoft 365 規範中心](https://protection.office.com/)。

2. 移至 [**搜尋**  >  **審核記錄搜尋**] 頁面。

3. 在 [ **開始日期** ] 和 [ **結束日期** ] 欄位中，選取日期範圍。

4. 在 [ **Exchange 信箱活動**] 底下，確認 [**活動**] 欄位設定為 **New-InboxRule 建立/修改/啟用/停用收件匣規則**。

5. 按一下 [搜尋]。

在結果中，選取一個審計記錄。 在 [詳細資料] 快顯視窗中，按一下 [ **詳細資訊**]。 [ **參數** ] 欄位中會顯示 [收件匣規則] 設定的相關資訊。

如需詳細資訊，請參閱 [判斷使用者是否建立收件匣規則](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
