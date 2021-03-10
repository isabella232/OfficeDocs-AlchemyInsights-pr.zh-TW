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
ms.openlocfilehash: 14d2c9b1fe6764f5cd3a5a968586a19a03b62694
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641509"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="e897f-102">還原被刪除的信箱</span><span class="sxs-lookup"><span data-stu-id="e897f-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="e897f-103">當使用者失去 Exchange Online 授權時，其信箱會保留30天，而且只要重新將授權指派給使用者，就能復原。</span><span class="sxs-lookup"><span data-stu-id="e897f-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
1. <span data-ttu-id="e897f-104">在 Microsoft 365 系統管理中心中，移至 [ **使用者** 作用中 \> **使用者** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="e897f-104">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="e897f-105">選取有問題的使用者。</span><span class="sxs-lookup"><span data-stu-id="e897f-105">Select the user in question.</span></span>

2. <span data-ttu-id="e897f-106">在 [ **授權與應用程式** ] 索引標籤上，指派 Exchange Online 授權，然後選取 [ **儲存變更**]。</span><span class="sxs-lookup"><span data-stu-id="e897f-106">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="e897f-107">如果您嘗試復原共用信箱或已刪除的使用者，它也可在30天內復原。</span><span class="sxs-lookup"><span data-stu-id="e897f-107">If you are trying to recover a shared mailbox or a user that was deleted, it is also recoverable for 30 days.</span></span> <span data-ttu-id="e897f-108">您可以在 [ **使用者** \> **刪除的使用者**] 底下找到這些使用者; 共用信箱不需要授權。</span><span class="sxs-lookup"><span data-stu-id="e897f-108">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="e897f-109">請參閱 [還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="e897f-109">Please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="e897f-110">從使用者的信箱復原電子郵件可以由系統管理員移至 [新的 Exchange 系統管理中心](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353)來完成。</span><span class="sxs-lookup"><span data-stu-id="e897f-110">Recovery of email from user's mailbox can be done by admins by going to the [new Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span></span>

<span data-ttu-id="e897f-111">最後，如果您嘗試復原非使用中的信箱，請 [依照這裡的指示](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox)進行。</span><span class="sxs-lookup"><span data-stu-id="e897f-111">Finally, if you are trying to recover an Inactive mailbox, [follow the instructions here](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span></span>
  
