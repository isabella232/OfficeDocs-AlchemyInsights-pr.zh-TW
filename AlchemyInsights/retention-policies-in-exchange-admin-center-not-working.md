---
title: Exchange 系統管理中心中的保留原則無法運作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369656"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 系統管理中心中的保留原則

 **問題:** Exchange 系統管理中心中新建立或更新的保留原則不會套用至信箱或專案不會移至封存信箱或刪除。 
  
 **根本原因:**
  
- 這可能是因為**受管理的資料夾助理**尚未處理使用者的信箱。 受管理的資料夾助理會嘗試每隔7天處理雲端架構組織中的每一個信箱。 如果您變更保留標記或將不同的保留原則套用至信箱, 您可以等到受管理的資料夾協助處理信箱, 或是執行 ManagedFolderAssistant 指令程式來啟動受管理的資料夾助理, 以處理特定的郵件. 執行此 Cmdlet 對於測試或疑難排解保留原則或保留標記設定很有用。 如需詳細資訊, 請造訪[執行受管理的資料夾助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **解決方案:** 執行下列命令, 為特定信箱啟動受管理的資料夾助理:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 如果已在信箱上啟用**RetentionHold** , 也**** 可能會發生這種情況。 如果信箱已放在 RetentionHold 中, 則在此期間不會處理信箱的保留原則。 如需 RetentionHold 設定的詳細 informaton, 請參閱:[信箱保留暫](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)止。
    
    **方法**
    
  - 檢查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定信箱上的 RetentionHold 設定狀態:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 執行下列命令, 以**停**用特定信箱上的 RetentionHold:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 現在, 請重新執行受管理的資料夾助理:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **附注:** 如果信箱小於 10 MB, 受管理的資料夾助理將不會自動處理信箱。
  