---
title: 無法使用 Exchange 系統管理中心中的保留原則
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761573"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="83bd1-102">在 Exchange 系統管理中心中的保留原則</span><span class="sxs-lookup"><span data-stu-id="83bd1-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="83bd1-103">**問題：** 新建立的 Exchange 系統管理中心中的已更新的保留原則不會套用到信箱或無法移至封存信箱或刪除項目。</span><span class="sxs-lookup"><span data-stu-id="83bd1-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="83bd1-104">**根本原因：**</span><span class="sxs-lookup"><span data-stu-id="83bd1-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="83bd1-105">這可能是因為**受管理的資料夾助理員**無法處理使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="83bd1-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="83bd1-106">受管理的資料夾助理員會嘗試處理雲端架構組織中一次每隔七天的每個信箱。</span><span class="sxs-lookup"><span data-stu-id="83bd1-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="83bd1-107">如果您變更的保留標記，或將不同的保留原則套用到信箱，您可以等到受管理資料夾助手處理信箱，或者您可以執行以啟動 [受管理的資料夾助理員處理特定 Start-managedfolderassistant 指令程式信箱。</span><span class="sxs-lookup"><span data-stu-id="83bd1-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="83bd1-108">執行此 cmdlet 可用於測試或疑難排解保留原則或保留標記設定。</span><span class="sxs-lookup"><span data-stu-id="83bd1-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="83bd1-109">如需詳細資訊，請造訪[執行受管理的資料夾助理員](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="83bd1-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="83bd1-110">**方案：** 執行下列命令，以啟動受管理的資料夾助理員特定信箱的：</span><span class="sxs-lookup"><span data-stu-id="83bd1-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="83bd1-111">此外，這也可能會發生如果**RetentionHold**已在信箱上的 [**已啟用**。</span><span class="sxs-lookup"><span data-stu-id="83bd1-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="83bd1-112">如果信箱具有已處於 RetentionHold，在這段期間將不會處理信箱的保留原則。</span><span class="sxs-lookup"><span data-stu-id="83bd1-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="83bd1-113">針對在 RetentionHold 設定，請參閱詳細資訊：[保留信箱保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。</span><span class="sxs-lookup"><span data-stu-id="83bd1-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="83bd1-114">**解決方案：**</span><span class="sxs-lookup"><span data-stu-id="83bd1-114">**Solution:**</span></span>
    
  - <span data-ttu-id="83bd1-115">檢查 RetentionHold 設定[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中的特定信箱的狀態：</span><span class="sxs-lookup"><span data-stu-id="83bd1-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="83bd1-116">在特定信箱上執行下列命令，以**停用**RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="83bd1-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="83bd1-117">現在，重新執行受管理的資料夾助理員：</span><span class="sxs-lookup"><span data-stu-id="83bd1-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="83bd1-118">**附註：** 如果信箱小於 10 MB，受管理的資料夾助理員不會自動處理的信箱。</span><span class="sxs-lookup"><span data-stu-id="83bd1-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

