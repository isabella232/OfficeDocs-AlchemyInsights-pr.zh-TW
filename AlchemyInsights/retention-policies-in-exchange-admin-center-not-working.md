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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371289"
---
# <a name="retention-policies-in-exchange-admin-center"></a>在 Exchange 系統管理中心中的保留原則

 **問題：** 新建立的 Exchange 系統管理中心中的已更新的保留原則不會套用到信箱或無法移至封存信箱或刪除項目。 
  
 **根本原因：**
  
- 這可能是因為**受管理的資料夾助理員**無法處理使用者的信箱。 受管理的資料夾助理員會嘗試處理雲端架構組織中一次每隔七天的每個信箱。 如果您變更的保留標記，或將不同的保留原則套用到信箱，您可以等到受管理資料夾助手處理信箱，或者您可以執行以啟動 [受管理的資料夾助理員處理特定 Start-managedfolderassistant 指令程式信箱。 執行此 cmdlet 可用於測試或疑難排解保留原則或保留標記設定。 如需詳細資訊，請造訪[執行受管理的資料夾助理員](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **方案：** 執行下列命令，以啟動受管理的資料夾助理員特定信箱的： 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 此外，這也可能會發生如果**RetentionHold**已在信箱上的 [**已啟用**。 如果信箱具有已處於 RetentionHold，在這段期間將不會處理信箱的保留原則。 針對在 RetentionHold 設定，請參閱詳細資訊：[保留信箱保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。
    
    **解決方案：**
    
  - 檢查 RetentionHold 設定[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中的特定信箱的狀態：
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 在特定信箱上執行下列命令，以**停用**RetentionHold: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 現在，重新執行受管理的資料夾助理員：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **附註：** 如果信箱小於 10 MB，受管理的資料夾助理員不會自動處理的信箱。 
  

