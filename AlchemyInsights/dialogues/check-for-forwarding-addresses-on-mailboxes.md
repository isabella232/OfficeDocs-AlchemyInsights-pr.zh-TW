---
title: 檢查信箱上的轉發位址
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417050"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="e12bf-102">檢查信箱上的轉發位址</span><span class="sxs-lookup"><span data-stu-id="e12bf-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="e12bf-103">有時候，駭客會將使用者的電子郵件轉寄給自己，所以先在信箱上檢查轉寄位址和規則。</span><span class="sxs-lookup"><span data-stu-id="e12bf-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="e12bf-104">然後，我們會檢查審核記錄檔。</span><span class="sxs-lookup"><span data-stu-id="e12bf-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="e12bf-105">以下說明如何檢查轉寄位址：</span><span class="sxs-lookup"><span data-stu-id="e12bf-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="e12bf-106">選取 [**使用者** 作用  >  中 **使用者**]。</span><span class="sxs-lookup"><span data-stu-id="e12bf-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="e12bf-107">選取其帳戶已遭破壞的使用者。</span><span class="sxs-lookup"><span data-stu-id="e12bf-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="e12bf-108">在出現的快顯視窗中，展開 [ **郵件設定**]，然後按一下 [ **編輯** ] 以進行 **電子郵件** 轉寄。</span><span class="sxs-lookup"><span data-stu-id="e12bf-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="e12bf-109">移除您不會辨識的任何轉寄位址。</span><span class="sxs-lookup"><span data-stu-id="e12bf-109">Remove any forwarding addresses you don't recognize.</span></span>