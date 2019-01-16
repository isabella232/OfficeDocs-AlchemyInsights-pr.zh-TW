---
title: 無法使用 Exchange 系統管理中心中的保留原則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278307"
---
 <span data-ttu-id="f3a8f-102">**問題：** 新建立的 Exchange 系統管理中心中的更新的保留原則不會套用至信箱或項目不會移到封存信箱或刪除。</span><span class="sxs-lookup"><span data-stu-id="f3a8f-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="f3a8f-103">**根本原因：**</span><span class="sxs-lookup"><span data-stu-id="f3a8f-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="f3a8f-p101">這可能是因為**受管理的資料夾助理員**無法處理使用者的信箱。受管理的資料夾助理員會嘗試處理雲端架構組織中一次每七天的每個信箱。如果您變更其保留標記或不同的保留原則套用到信箱，您可以等候受管理的資料夾協助處理的信箱，或者您可以執行以啟動受管理的資料夾助理員處理特定 Start-managedfolderassistant 指令程式信箱。執行此指令程式是適用於測試或疑難排解保留原則或保留標記設定。如需詳細資訊，請造訪[受管理的資料夾助理員執行](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="f3a8f-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="f3a8f-109">**解決方案：** 執行下列命令以啟動受管理的資料夾助理員特定信箱：</span><span class="sxs-lookup"><span data-stu-id="f3a8f-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="f3a8f-p102">這也可能會發生如果**RetentionHold**已在信箱上的 [**已啟用**。如果 RetentionHold 上放置信箱、 信箱的保留原則將不會處理的時間。針對 RetentionHold 設定請參閱上的詳細資訊：[信箱保留](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。</span><span class="sxs-lookup"><span data-stu-id="f3a8f-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="f3a8f-113">**解決方案：**</span><span class="sxs-lookup"><span data-stu-id="f3a8f-113">**Solution:**</span></span>
    
  - <span data-ttu-id="f3a8f-114">檢查 RetentionHold 信箱上設定特定[EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中的狀態：</span><span class="sxs-lookup"><span data-stu-id="f3a8f-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="f3a8f-115">在特定的信箱上執行下列命令以**停用**RetentionHold：</span><span class="sxs-lookup"><span data-stu-id="f3a8f-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="f3a8f-116">現在，重新執行受管理資料夾助理：</span><span class="sxs-lookup"><span data-stu-id="f3a8f-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="f3a8f-117">**附註：** 如果信箱小於 10 MB，受管理的資料夾助理員會自動處理信箱。</span><span class="sxs-lookup"><span data-stu-id="f3a8f-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

