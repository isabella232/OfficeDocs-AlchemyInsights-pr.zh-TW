---
title: 還原已刪除的信箱
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
ms.openlocfilehash: 92761e4679a155781555daec023ee9602d62a857
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356084"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="2b64c-102">還原被刪除的信箱</span><span class="sxs-lookup"><span data-stu-id="2b64c-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="2b64c-103">當使用者失去其 Exchange Online 授權時, 其信箱會保留30天, 而且只要重新指派授權給使用者, 即可進行復原。</span><span class="sxs-lookup"><span data-stu-id="2b64c-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="2b64c-104">*這只會在30天內運作。*</span><span class="sxs-lookup"><span data-stu-id="2b64c-104">*This will work only within 30 days.*</span></span>  <span data-ttu-id="2b64c-105">在管理入口網站中, 移至:</span><span class="sxs-lookup"><span data-stu-id="2b64c-105">In the Admin Portal, go to:</span></span>
  
1. <span data-ttu-id="2b64c-106">**使用者**\> \*\*\*\* 作用中的使用者。</span><span class="sxs-lookup"><span data-stu-id="2b64c-106">**Users** \> **Active** users.</span></span> <span data-ttu-id="2b64c-107">選取 [有問題的使用者]。</span><span class="sxs-lookup"><span data-stu-id="2b64c-107">Select the user in question.</span></span>

2. <span data-ttu-id="2b64c-108">按 [**編輯**] 修改產品授權</span><span class="sxs-lookup"><span data-stu-id="2b64c-108">Press **Edit** to modify Product licenses</span></span>

3. <span data-ttu-id="2b64c-109">指派 Exchange Online 授權, 然後按 [**儲存**]</span><span class="sxs-lookup"><span data-stu-id="2b64c-109">Assign the Exchange Online license and press **Save**</span></span>

<span data-ttu-id="2b64c-110">如果您嘗試復原共用信箱, 它也可在30天內復原。</span><span class="sxs-lookup"><span data-stu-id="2b64c-110">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="2b64c-111">您可以在 [**使用者** \> **已刪除**的使用者] 底下找到它們。共用信箱不需要授權。</span><span class="sxs-lookup"><span data-stu-id="2b64c-111">You can find them under **Users** \> **Deleted** users; shared mailboxes do not require a license.</span></span> <span data-ttu-id="2b64c-112">如果您意識到您需要還原已刪除的使用者, 請參閱[restore a user In Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="2b64c-112">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user).</span></span>
  