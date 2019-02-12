---
title: 無法使用 Exchange 系統管理中心中的保留原則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934983"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 系統管理中心中的保留原則

 **問題：** 新建立的 Exchange 系統管理中心中的更新的保留原則不會套用至信箱或項目不會移到封存信箱或刪除。 
  
 **根本原因：**
  
- 這可能是因為**受管理的資料夾助理員**無法處理使用者的信箱。受管理的資料夾助理員會嘗試處理雲端架構組織中一次每七天的每個信箱。如果您變更其保留標記或不同的保留原則套用到信箱，您可以等候受管理的資料夾協助處理的信箱，或者您可以執行以啟動受管理的資料夾助理員處理特定 Start-managedfolderassistant 指令程式信箱。執行此指令程式是適用於測試或疑難排解保留原則或保留標記設定。如需詳細資訊，請造訪[受管理的資料夾助理員執行](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **解決方案：** 執行下列命令以啟動受管理的資料夾助理員特定信箱： 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 這也可能會發生如果**RetentionHold**已在信箱上的 [**已啟用**。如果 RetentionHold 上放置信箱、 信箱的保留原則將不會處理的時間。針對 RetentionHold 設定請參閱上的詳細資訊：[信箱保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。
    
    **解決方案：**
    
  - 檢查 RetentionHold 信箱上設定特定[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中的狀態：
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 在特定的信箱上執行下列命令以**停用**RetentionHold： 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 現在，重新執行受管理資料夾助理：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **附註：** 如果信箱小於 10 MB，受管理的資料夾助理員會自動處理信箱。 
  

