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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464438"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>瞭解誰會在信箱上設定轉發，以及如何

如果在信箱上設定外部轉寄，該活動會在 Set-Mailbox Cmdlet 中進行審核。 以下說明如何在審計記錄檔中尋找活動：

1. 移至 [Office 365 的安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 選取 [**搜尋** >  **審核記錄搜尋**]。
    > [!NOTE]
    > 如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。 若未開啟此功能，搜尋結果將無法從先前的日期提取資料。
1. 請確定 [ **活動** ] 欄位已設定為顯示預設)  (**所有活動的結果** 。 指定日期範圍。 您不需要指定使用者名稱。
1. 選取 [ **搜尋**]。 活動會顯示在 [ **結果**] 底下。
1. 選取 [**篩選結果**]，然後在 [**活動** 篩選] 欄位中輸入 **集信箱**。 這會傳回所有的 **Set-Mailbox** 活動。
1. 若要查看詳細資料，請選取活動，然後選取 [ **詳細資訊**]。 在 [ **參數** ] 底下您可以看到信箱上設定的轉寄電子郵件地址。 **UserID** 代表在信箱上設定外部轉送的使用者。
若要深入瞭解，請參閱 [搜尋 Office 365 audit log 以進行常見案例疑難排解](https://go.microsoft.com/fwlink/?linkid=2103944)。