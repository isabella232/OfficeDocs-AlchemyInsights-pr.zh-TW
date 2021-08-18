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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331150"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>識別信箱上設定外部電子郵件轉寄的時間

當 Microsoft 365 使用者設定信箱上的外部電子郵件轉寄功能時，會在 **Set-Mailbox** Cmdlet 中審核該活動。 您可以使用 [審計記錄檔] 搜尋來查看活動。 以下說明如何執行。

1. 執行下列其中一個步驟：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://sip.security.microsoft.com/auditlogsearch> 。

2. 在 [ **審計** ] 頁面上，確認已選取 [ **搜尋] 索引** 標籤，然後設定下列設定：
   - 選取 [ **開始** ] 和 [ **結束** ] 方塊中的日期/時間範圍。
   - 確認 [ **活動** ] 方塊中包含 **所有活動的顯示結果**。

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 在結果中，按一下 [ **篩選結果** ]，然後在 [活動篩選] 方塊中輸入 **Set-Mailbox** 。

5. 選取結果中的審計記錄。 在 [ **詳細資料** ] 快顯視窗中，按一下 [ **詳細資訊**]。 您必須查看每個審計記錄的詳細資料，以判斷活動是否與電子郵件轉寄有關。

   - **ObjectId**：已修改之信箱的別名值。
   - **參數**： _ForwardingSmtpAddress_ 表示目標電子郵件地址。
   - **UserId**：在 **ObjectId** 欄位中的信箱上設定電子郵件轉寄的使用者。

如需詳細資訊，請參閱 [決定誰設定信箱的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)轉寄功能。
