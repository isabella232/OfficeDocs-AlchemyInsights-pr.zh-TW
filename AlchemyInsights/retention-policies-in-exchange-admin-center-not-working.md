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
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740501"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 系統管理中心中的保留原則

如果您想讓我們為下列所述的設定執行自動檢查，請選取此頁面頂端的 [上一步] 按鈕 <--然後輸入具有保留原則問題的使用者電子郵件地址。

 **問題：** 在 Exchange 系統管理中心中新建立或更新的保留原則不會套用到信箱或專案，也不會移至封存信箱或已刪除。 
  
 **根源：**
  
- 這可能是因為 **受管理的資料夾助理** 尚未處理使用者的信箱。 受管理的資料夾助理每隔7天會嘗試處理雲端架構組織中的每個信箱。 如果您變更保留標記或將不同的保留原則套用至信箱，您可以等到受管理的資料夾協助處理該信箱，或執行 Start-ManagedFolderAssistant Cmdlet 以啟動受管理的資料夾助理來處理特定的信箱。 在測試或疑難排解保留原則或保留標記設定時，執行此 Cmdlet 很有用。 如需詳細資訊，請造訪 [執行受管理的資料夾助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **解決方案：** 執行下列命令，以啟動特定信箱的受管理的資料夾助理：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 如果已在信箱上啟用**RetentionHold** ，也**enabled**可能會發生這種情況。 如果信箱已放在 RetentionHold 中，信箱的保留原則在該時段內將不會被處理。 如需 RetentionHold 設定上的更多 informaton，請參閱： [信箱保留暫](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)止。
    
    **解決 方案：**
    
  - 檢查 [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定信箱上的 RetentionHold 設定狀態。
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 執行下列命令以 **停** 用特定信箱上的 RetentionHold：
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 現在，請重新執行受管理的資料夾助理：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **附注：** 如果信箱小於 10 MB，受管理的資料夾助理將不會自動處理信箱。
 
如需 Exchange 系統管理中心內保留原則的詳細資訊，請參閱：
- [保留標記和保留原則](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [將保留原則套用至信箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [新增或移除保留標記](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [如何找出位於信箱的保留類型](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
