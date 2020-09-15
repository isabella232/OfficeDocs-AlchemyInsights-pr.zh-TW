---
title: 在審核記錄中識別信箱上的外部電子郵件轉發
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696288"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>識別信箱上設定外部電子郵件轉寄的時間

當 Microsoft 365 使用者設定信箱上的外部電子郵件轉寄功能時，會在 **Set-Mailbox** Cmdlet 中審核該活動。 您可以在安全性 & 規範中心內，看到使用審核記錄搜尋的活動。

1. 登入 [Microsoft 365 的安全性 & 規範中心](https://protection.office.com/)。

2. 移至 [**搜尋**  >  **審核記錄搜尋**] 頁面。

3. 在 [ **開始日期** ] 和 [ **結束日期** ] 欄位中，選取日期範圍。 您不需要指定使用者名稱。 確認 [ **活動** ] 欄位已設定為 **顯示所有活動的結果**。

4. 按一下 [搜尋]。

在結果中，按一下 [ **篩選結果** ]，然後在 [活動篩選] 方塊中輸入 **Set-Mailbox** 。 選取結果中的審計記錄。 在 [ **詳細資料** ] 快顯視窗中，按一下 [ **詳細資訊**]。 您必須查看每個審計記錄的詳細資料，以判斷該活動是否與電子郵件轉寄有關。

- **ObjectId**：已修改之信箱的別名值。

- **參數**： _ForwardingSmtpAddress_ 表示目標電子郵件地址。

- **UserId**：在 **ObjectId** 欄位中的信箱上設定電子郵件轉寄的使用者。

如需詳細資訊，請參閱 [決定誰設定信箱的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)轉寄功能。
