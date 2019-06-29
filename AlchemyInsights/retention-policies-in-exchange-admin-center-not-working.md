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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="050e1-102">Exchange 系統管理中心中的保留原則</span><span class="sxs-lookup"><span data-stu-id="050e1-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="050e1-103">**問題:** Exchange 系統管理中心中新建立或更新的保留原則不會套用至信箱或專案不會移至封存信箱或刪除。</span><span class="sxs-lookup"><span data-stu-id="050e1-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="050e1-104">**根本原因:**</span><span class="sxs-lookup"><span data-stu-id="050e1-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="050e1-105">這可能是因為**受管理的資料夾助理**尚未處理使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="050e1-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="050e1-106">受管理的資料夾助理會嘗試每隔7天處理雲端架構組織中的每一個信箱。</span><span class="sxs-lookup"><span data-stu-id="050e1-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="050e1-107">如果您變更保留標記或將不同的保留原則套用至信箱, 您可以等到受管理的資料夾協助處理信箱, 或是執行 ManagedFolderAssistant 指令程式來啟動受管理的資料夾助理, 以處理特定的郵件.</span><span class="sxs-lookup"><span data-stu-id="050e1-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="050e1-108">執行此 Cmdlet 對於測試或疑難排解保留原則或保留標記設定很有用。</span><span class="sxs-lookup"><span data-stu-id="050e1-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="050e1-109">如需詳細資訊, 請造訪[執行受管理的資料夾助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="050e1-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="050e1-110">**解決方案:** 執行下列命令, 為特定信箱啟動受管理的資料夾助理:</span><span class="sxs-lookup"><span data-stu-id="050e1-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="050e1-111">如果已在信箱上啟用**RetentionHold** , 也\*\*\*\* 可能會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="050e1-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="050e1-112">如果信箱已放在 RetentionHold 中, 則在此期間不會處理信箱的保留原則。</span><span class="sxs-lookup"><span data-stu-id="050e1-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="050e1-113">如需 RetentionHold 設定的詳細 informaton, 請參閱:[信箱保留暫](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)止。</span><span class="sxs-lookup"><span data-stu-id="050e1-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="050e1-114">**方法**</span><span class="sxs-lookup"><span data-stu-id="050e1-114">**Solution:**</span></span>
    
  - <span data-ttu-id="050e1-115">檢查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定信箱上的 RetentionHold 設定狀態:</span><span class="sxs-lookup"><span data-stu-id="050e1-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="050e1-116">執行下列命令, 以**停**用特定信箱上的 RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="050e1-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="050e1-117">現在, 請重新執行受管理的資料夾助理:</span><span class="sxs-lookup"><span data-stu-id="050e1-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="050e1-118">**附注:** 如果信箱小於 10 MB, 受管理的資料夾助理將不會自動處理信箱。</span><span class="sxs-lookup"><span data-stu-id="050e1-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
  