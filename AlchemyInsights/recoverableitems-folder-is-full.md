---
title: 1336 RecoverableItems 資料夾已滿
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: a048949d5284d018303d03aad26cdf26eee2fb5c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776388"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="bee62-102">[可復原的項目] 資料夾已滿</span><span class="sxs-lookup"><span data-stu-id="bee62-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="bee62-103">在 Office 365 中的 Exchange Online 信箱，[可復原的項目] 資料夾的預設儲存量限制為 30 GB。</span><span class="sxs-lookup"><span data-stu-id="bee62-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="bee62-104">如果信箱處於訴訟暫止狀態，eDiscovery 保留] 中，或指派給 Office 365 保留原則，[可復原的項目] 資料夾的儲存量限制會自動增加到 100GB。</span><span class="sxs-lookup"><span data-stu-id="bee62-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="bee62-105">當 [可復原的項目] 資料夾達到儲存量限制時，是以下列方式影響信箱功能：</span><span class="sxs-lookup"><span data-stu-id="bee62-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="bee62-106">使用者無法從信箱中刪除項目。</span><span class="sxs-lookup"><span data-stu-id="bee62-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="bee62-107">受管理的資料夾助理員無法刪除保留標記或受管理的資料夾設定為基礎的項目。</span><span class="sxs-lookup"><span data-stu-id="bee62-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="bee62-108">啟用單一項目復原或會處於保留狀態的信箱，寫入時複製頁面保護程序無法維護版本的使用者編輯項目。</span><span class="sxs-lookup"><span data-stu-id="bee62-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="bee62-109">針對已啟用信箱稽核記錄的信箱，沒有信箱稽核記錄項目可以儲存在 [可復原的項目] 資料夾中的 [稽核] 子資料夾中。</span><span class="sxs-lookup"><span data-stu-id="bee62-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="bee62-110">針對不保留的信箱，系統管理員可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent`命令在 Exchange Online PowerShell 中刪除 [可復原的項目] 資料夾中的項目。</span><span class="sxs-lookup"><span data-stu-id="bee62-110">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="bee62-111">如需相關資訊，請參閱下列主題：</span><span class="sxs-lookup"><span data-stu-id="bee62-111">For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="bee62-112">搜尋並刪除郵件</span><span class="sxs-lookup"><span data-stu-id="bee62-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="bee62-113">搜尋信箱</span><span class="sxs-lookup"><span data-stu-id="bee62-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="bee62-114">針對要保留的信箱，系統管理員必須移除保留，他們可以從 [可復原的項目] 資料夾刪除項目之前。</span><span class="sxs-lookup"><span data-stu-id="bee62-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="bee62-115">如需詳細資訊，請參閱 <<c0>可復原的項目保留的雲端架構信箱上的資料夾內刪除項目。</span><span class="sxs-lookup"><span data-stu-id="bee62-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="bee62-116">若要協助防止成為完整 [可復原的項目] 資料夾，系統管理員可以增加可復原的項目資料夾信箱的保留和設定將項目從 [可復原的項目] 資料夾移至使用者的封存的信箱保留原則的儲存限制信箱。</span><span class="sxs-lookup"><span data-stu-id="bee62-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="bee62-117">請參閱[增加可復原的項目配額的信箱保留](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。</span><span class="sxs-lookup"><span data-stu-id="bee62-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

