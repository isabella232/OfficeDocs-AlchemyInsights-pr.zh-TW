---
title: 識別在稽核記錄中的信箱上的外部電子郵件轉寄
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909085"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>找出何時會在信箱上設定外部電子郵件轉寄

當使用者在信箱上設定外部電子郵件轉寄時，活動被稽核**Set-mailbox**指令程式的一部分。 您可以查看使用中的安全性 & 合規性中心的稽核記錄搜尋的活動。

1. 登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)

2. 按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。

3. 在 [**開始日期**和**結束日期**] 欄位中選取日期範圍。 您不需要指定使用者名稱。 確認 [**活動**] 欄位設為**顯示結果的所有活動**。

4. Click **Search**.

在結果中，按一下**篩選結果**，在 [活動篩選] 方塊中輸入**Set-mailbox** 。 在結果中，選取 [稽核記錄。 在**詳細資料**彈出式視窗中，按一下 [**更多的資訊**。 您必須將看的每個稽核記錄，以判斷活動是否與電子郵件轉寄功能的相關詳細資料。

- **ObjectId**： 上次修改信箱的別名值。

- **參數**： _ForwardingSmtpAddress_指出目標電子郵件地址。

- **UserId**: **ObjectId**欄位中信箱設定電子郵件轉寄功能的使用者。

如需詳細資訊，請參閱 <<c0>的判斷設定電子郵件轉寄的信箱。
