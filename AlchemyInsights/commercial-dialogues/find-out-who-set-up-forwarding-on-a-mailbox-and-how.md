---
title: 瞭解誰會在信箱上設定轉發，以及如何
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317799"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>瞭解誰會在信箱上設定轉發，以及如何

如果在信箱上設定外部轉寄，該活動會在 **Set-Mailbox** Cmdlet 中進行審核。 以下說明如何在審計記錄檔中尋找活動：

1. 請執行下列其中一個動作：
   - 在 Microsoft 365 合規性中心 <https://compliance.microsoft.com> ，移至 [**解決方案** \> **審核**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**審計**]。 或者，若要直接移至 [ **審計** ] 頁面，請使用 <https://security.microsoft.com/auditlogsearch> 。

   **附注**：如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。 若未開啟此功能，搜尋結果將無法從先前的日期提取資料。

2. 在 [ **審計** ] 頁面上，確認已選取 [ **搜尋] 索引** 標籤，然後設定下列設定：
   - 選取 [ **開始** ] 和 [ **結束** ] 方塊中的日期/時間範圍。
   - 確認 [ **活動** ] 方塊中包含 **所有活動的顯示結果**。

3. 完成後，請按一下 [ **搜尋**]。 活動會顯示在 [新的 **審計搜尋** ] 頁面上。

4. 在結果中，按一下 [ **活動** ] 欄，以排序結果，並尋找 **Set-Mailbox** 專案。

5. 選取結果中的活動，以開啟 [詳細資料] 快顯視窗。 您必須查看每個審計記錄的詳細資料，以判斷活動是否與電子郵件轉寄有關：
   - **ObjectId**：已修改之信箱的別名值。
   - **參數**： _ForwardingSmtpAddress_ 表示目標電子郵件地址。
   - **UserId**：在 **ObjectId** 欄位中的信箱上設定電子郵件轉寄的使用者。

如需詳細資訊，請參閱 [決定誰設定信箱的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)轉寄功能。
