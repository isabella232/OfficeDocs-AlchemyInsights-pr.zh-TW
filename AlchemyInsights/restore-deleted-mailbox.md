---
title: 還原已刪除的信箱
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 899eb7e171d125c509871c219f99dfd1106b858a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728062"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="b9fc6-102">還原被刪除的信箱</span><span class="sxs-lookup"><span data-stu-id="b9fc6-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="b9fc6-103">當使用者失去 Exchange Online 授權時，其信箱會保留30天，而且只要重新將授權指派給使用者，就能復原。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="b9fc6-104">*這只會在30天內運作。*</span><span class="sxs-lookup"><span data-stu-id="b9fc6-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="b9fc6-105">在 Microsoft 365 系統管理中心中，移至 [ **使用者**作用中 \> **使用者** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="b9fc6-106">選取有問題的使用者。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-106">Select the user in question.</span></span>

2. <span data-ttu-id="b9fc6-107">在 [ **授權與應用程式** ] 索引標籤上，指派 Exchange Online 授權，然後選取 [ **儲存變更**]。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="b9fc6-108">如果您嘗試復原共用信箱，它也可在30天內復原。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="b9fc6-109">您可以在 [ **使用者** \> **刪除的使用者**] 底下找到這些使用者; 共用信箱不需要授權。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="b9fc6-110">如果您知道需要還原已刪除的使用者，請參閱 [還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="b9fc6-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  