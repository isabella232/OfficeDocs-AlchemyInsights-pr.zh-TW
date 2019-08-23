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
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 9fc1980b5c1d5a0bd9df032b14e2010b7f0d5873
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551838"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="46376-102">還原被刪除的信箱</span><span class="sxs-lookup"><span data-stu-id="46376-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="46376-103">當使用者將會遺失其 Exchange Online 授權時，他們的信箱會保留 30 天，並可復原只需要重新指派授權給使用者。</span><span class="sxs-lookup"><span data-stu-id="46376-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="46376-104">*只有在 30 天內運作。*</span><span class="sxs-lookup"><span data-stu-id="46376-104">*This will work only within 30 days.*</span></span>  <span data-ttu-id="46376-105">在系統管理入口網站中，移至：</span><span class="sxs-lookup"><span data-stu-id="46376-105">In the Admin Portal, go to:</span></span>
  
1. <span data-ttu-id="46376-106">**使用者**\> **作用中**的使用者。</span><span class="sxs-lookup"><span data-stu-id="46376-106">**Users** \> **Active** users.</span></span> <span data-ttu-id="46376-107">選取有問題的使用者。</span><span class="sxs-lookup"><span data-stu-id="46376-107">Select the user in question.</span></span>

2. <span data-ttu-id="46376-108">按 [**編輯**]，以修改產品授權</span><span class="sxs-lookup"><span data-stu-id="46376-108">Press **Edit** to modify Product licenses</span></span>

3. <span data-ttu-id="46376-109">指派 Exchange Online 授權，然後按 [**儲存**</span><span class="sxs-lookup"><span data-stu-id="46376-109">Assign the Exchange Online license and press **Save**</span></span>

<span data-ttu-id="46376-110">如果您嘗試復原共用信箱，它也是 [可復原的 30 天。</span><span class="sxs-lookup"><span data-stu-id="46376-110">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="46376-111">您可以在 [**使用者]** 找到\>**已刪除**的使用者;共用的信箱不需要授權。</span><span class="sxs-lookup"><span data-stu-id="46376-111">You can find them under **Users** \> **Deleted** users; shared mailboxes do not require a license.</span></span> <span data-ttu-id="46376-112">如果您知道您需要還原已刪除的使用者，請參閱[還原 Office 365 中的使用者](https://docs.microsoft.com/office365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="46376-112">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  