---
title: Exchange Admin Center 中的保留原則無法運作
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952219"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 系統管理中心中的保留原則

如果您想讓我們為下列所述的設定執行自動檢查，請選取此頁面頂端的 [上一步] 按鈕 <--然後輸入具有保留原則問題的使用者電子郵件地址。

如果您在 Exchange 系統管理中心中的保留原則發生問題，但未套用到信箱或專案不會移至封存信箱，請檢查下列事項：

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
