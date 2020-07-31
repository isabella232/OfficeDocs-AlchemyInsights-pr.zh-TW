---
title: Exchange Admin Center 中的保留原則無法運作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522798"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="0f493-102">Exchange 系統管理中心中的保留原則</span><span class="sxs-lookup"><span data-stu-id="0f493-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="0f493-103">如果您想讓我們為下列所述的設定執行自動檢查，請選取此頁面頂端的 [上一步] 按鈕 <--然後輸入具有保留原則問題的使用者電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="0f493-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="0f493-104">**問題：** 在 Exchange 系統管理中心中新建立或更新的保留原則不會套用到信箱或專案，也不會移至封存信箱或已刪除。</span><span class="sxs-lookup"><span data-stu-id="0f493-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="0f493-105">**根源：**</span><span class="sxs-lookup"><span data-stu-id="0f493-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="0f493-106">這可能是因為**受管理的資料夾助理**尚未處理使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="0f493-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="0f493-107">受管理的資料夾助理每隔7天會嘗試處理雲端架構組織中的每個信箱。</span><span class="sxs-lookup"><span data-stu-id="0f493-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="0f493-108">如果您變更保留標記或將不同的保留原則套用至信箱，您可以等到受管理的資料夾協助處理該信箱，或執行 Start-ManagedFolderAssistant Cmdlet 以啟動受管理的資料夾助理來處理特定的信箱。</span><span class="sxs-lookup"><span data-stu-id="0f493-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="0f493-109">在測試或疑難排解保留原則或保留標記設定時，執行此 Cmdlet 很有用。</span><span class="sxs-lookup"><span data-stu-id="0f493-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="0f493-110">如需詳細資訊，請造訪[執行受管理的資料夾助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="0f493-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="0f493-111">**解決方案：** 執行下列命令，以啟動特定信箱的受管理的資料夾助理：</span><span class="sxs-lookup"><span data-stu-id="0f493-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="0f493-112">如果已在信箱上啟用**RetentionHold** ，也**enabled**可能會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="0f493-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="0f493-113">如果信箱已放在 RetentionHold 中，信箱的保留原則在該時段內將不會被處理。</span><span class="sxs-lookup"><span data-stu-id="0f493-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="0f493-114">如需 RetentionHold 設定上的更多 informaton，請參閱：[信箱保留暫](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)止。</span><span class="sxs-lookup"><span data-stu-id="0f493-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="0f493-115">**解決 方案：**</span><span class="sxs-lookup"><span data-stu-id="0f493-115">**Solution:**</span></span>
    
  - <span data-ttu-id="0f493-116">檢查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定信箱上的 RetentionHold 設定狀態。</span><span class="sxs-lookup"><span data-stu-id="0f493-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="0f493-117">執行下列命令以**停**用特定信箱上的 RetentionHold：</span><span class="sxs-lookup"><span data-stu-id="0f493-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="0f493-118">現在，請重新執行受管理的資料夾助理：</span><span class="sxs-lookup"><span data-stu-id="0f493-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="0f493-119">**附注：** 如果信箱小於 10 MB，受管理的資料夾助理將不會自動處理信箱。</span><span class="sxs-lookup"><span data-stu-id="0f493-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="0f493-120">如需 Exchange 系統管理中心內保留原則的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="0f493-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="0f493-121">保留標記和保留原則</span><span class="sxs-lookup"><span data-stu-id="0f493-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="0f493-122">將保留原則套用至信箱</span><span class="sxs-lookup"><span data-stu-id="0f493-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="0f493-123">新增或移除保留標記</span><span class="sxs-lookup"><span data-stu-id="0f493-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="0f493-124">如何找出位於信箱的保留類型</span><span class="sxs-lookup"><span data-stu-id="0f493-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
