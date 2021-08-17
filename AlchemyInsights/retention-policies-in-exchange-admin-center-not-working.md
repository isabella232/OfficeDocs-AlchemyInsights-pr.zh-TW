---
title: Exchange 系統管理中心的保留原則無法運作
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074923"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 系統管理中心的保留原則

如果您想讓我們為下列所述的設定執行自動檢查，請選取此頁面頂端的 [上一步] 按鈕 <--然後輸入具有保留原則問題的使用者電子郵件地址。

如果您遇到 Exchange 系統管理中心的保留原則問題，但未套用到信箱或專案不會移至封存信箱，請檢查下列事項：

**根源：**

- **受管理的資料夾助理** 尚未處理使用者的信箱。 受管理的資料夾助理每隔7天會嘗試處理雲端架構組織中的每個信箱。

  **解決方案：** 執行受管理的資料夾助理。

- 信箱上已 **啟用** **RetentionHold** 。 如果信箱已放在 RetentionHold 中，信箱的保留原則在該時段內將不會被處理。

  **解決方案：** 檢查 [保留暫止] 設定的狀態，並視需要更新。 如需詳細資訊，請參閱 [信箱保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)功能。
 
**附注：** 如果信箱小於 10 MB，受管理的資料夾助理將不會自動處理信箱。
 
如需 Exchange 系統管理中心內保留原則的詳細資訊，請參閱：

- [保留標記和保留原則](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [將保留原則套用至信箱，](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 或 [新增或移除保留標記](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [如何找出位於信箱的保留類型](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
