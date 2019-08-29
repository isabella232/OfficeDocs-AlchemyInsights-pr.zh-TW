---
title: 還原已刪除信箱
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
ms.openlocfilehash: 44b23be5e75a0669821bbeb07b0f064eeef6d021
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666363"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="1c3a0-102">還原被刪除的信箱</span><span class="sxs-lookup"><span data-stu-id="1c3a0-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="1c3a0-103">當使用者將會遺失的 Exchange Online 授權時，他們的信箱會保留 30 天，並可復原只需要重新指派授權給使用者。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="1c3a0-104">*只有在 30 天內運作。*</span><span class="sxs-lookup"><span data-stu-id="1c3a0-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="1c3a0-105">在 Microsoft 365 系統管理中心，移至 [**使用者** \> **作用中使用者**頁面。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="1c3a0-106">選取有問題的使用者。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-106">Select the user in question.</span></span>

2. <span data-ttu-id="1c3a0-107">在 [**授權及應用程式**] 索引標籤上指派 Exchange Online 授權然後選取 [**儲存變更**。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="1c3a0-108">如果您嘗試復原共用信箱，它也是 [可復原的 30 天。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="1c3a0-109">您可以在 [**使用者]** 找到\>**已刪除使用者**。共用的信箱不需要授權。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="1c3a0-110">如果您知道您需要還原已刪除的使用者，請參閱[還原 Office 365 中的使用者](https://docs.microsoft.com/office365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="1c3a0-110">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  