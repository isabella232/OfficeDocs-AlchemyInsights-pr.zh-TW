---
title: 還原已刪除信箱
ms.author: pebaum
author: pebaum
ms.date: 9/12/2017
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: da3d35e5f86f2b76fe6bd25829458b1b2d1a1e9a
ms.sourcegitcommit: c3ed7525f24f80cc6372aa3f496463500bb0c3ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/19/2019
ms.locfileid: "30088104"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="dfc5f-102">還原被刪除的信箱</span><span class="sxs-lookup"><span data-stu-id="dfc5f-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="dfc5f-103">當使用者將會遺失其 Exchange Online 授權時，他們的信箱會保留 30 天和可復原只需要重新指派授權給使用者。</span><span class="sxs-lookup"><span data-stu-id="dfc5f-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="dfc5f-p101">*這會運作 30 天內只有。* 在系統入口網站中，移至：</span><span class="sxs-lookup"><span data-stu-id="dfc5f-p101">*This will work only within 30 days.*  In the Admin Portal, go to:</span></span> 
  
1. <span data-ttu-id="dfc5f-p102">**使用者**\> **作用中**使用者。選取有問題的使用者。</span><span class="sxs-lookup"><span data-stu-id="dfc5f-p102">**Users** \> **Active** users. Select the user in question.</span></span> 
    
2. <span data-ttu-id="dfc5f-108">按 [**編輯**] 以修改產品授權</span><span class="sxs-lookup"><span data-stu-id="dfc5f-108">Press **Edit** to modify Product licenses</span></span> 
    
3. <span data-ttu-id="dfc5f-109">指派 Exchange Online 授權和按**儲存**</span><span class="sxs-lookup"><span data-stu-id="dfc5f-109">Assign the Exchange Online license and press **Save**</span></span>
    
<span data-ttu-id="dfc5f-p103">如果您嘗試復原共用信箱，也有可復原的 30 天。您可以找到這些**使用者**底下\> **Deleted**使用者;共用的信箱不需要授權。如果您知道您需要還原已刪除的使用者，請參閱[還原 Office 365 中的使用者](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="dfc5f-p103">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days. You can find them under **Users** \> **Deleted** users; shared mailboxes do not require a license. If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user).</span></span>
  

