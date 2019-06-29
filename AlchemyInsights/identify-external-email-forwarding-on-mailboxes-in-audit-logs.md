---
title: 在審計記錄檔中識別信箱上的外部電子郵件轉寄
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383088"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>識別信箱上設定外部電子郵件轉寄的時機

當使用者在信箱上設定外部電子郵件轉寄時, 會將活動作為**設定信箱指令程式**的一部分進行審核。 您可以在安全性 & 規範中心內使用 [審核記錄搜尋] 來查看活動。

1. 登入[Office 365 安全性 & 規範中心](https://protection.office.com/)

2. 按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。

3. 選取 [**開始日期**] 和 [**結束日期**] 欄位中的日期範圍。 您不需要指定使用者名稱。 確認 [**活動**] 欄位已設為 [**顯示所有活動的結果**]。

4. Click **Search**.

在結果中, 按一下 [**篩選結果**], 然後在 [活動篩選] 方塊中輸入**集-信箱**。 在結果中選取一筆審計記錄。 在 [**詳細資料**] 快顯視窗中, 按一下 [**詳細資訊**]。 您必須查看每個審計記錄的詳細資料, 以判斷活動是否與電子郵件轉寄有關。

- **ObjectId**: 已修改之信箱的別名值。

- **參數**: _ForwardingSmtpAddress_指出目標電子郵件地址。

- **UserId**: 在 [ **ObjectId** ] 欄位的信箱上設定電子郵件轉寄的使用者。

如需詳細資訊, 請參閱[決定如何設定信箱的電子郵件](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)轉寄功能。
