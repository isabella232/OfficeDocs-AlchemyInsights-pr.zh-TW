---
title: 修正使用者原則/信箱設定
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568498"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="9372f-102">修正使用者原則/信箱設定</span><span class="sxs-lookup"><span data-stu-id="9372f-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="9372f-103">信箱上的垃圾郵件設定會影響此郵件。</span><span class="sxs-lookup"><span data-stu-id="9372f-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="9372f-104">若要複查設定，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="9372f-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="9372f-105">啟動 Exchange 管理命令介面。</span><span class="sxs-lookup"><span data-stu-id="9372f-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="9372f-106">如需詳細資訊，請參閱 [開啟 Exchange 管理命令](https://go.microsoft.com/fwlink/?linkid=2101432)介面。</span><span class="sxs-lookup"><span data-stu-id="9372f-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="9372f-107">使用使用者的電子郵件地址執行此命令 () ：  **mailboxjunkmailconfiguration-identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="9372f-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="9372f-108">檢查寄件者的電子郵件地址是否屬於 **TrustedSendersAndDomains** 或 **BlockedSendersAndDomains**。</span><span class="sxs-lookup"><span data-stu-id="9372f-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="9372f-109">如果電子郵件地址位於其中一個清單中，您可能必須加以移除。</span><span class="sxs-lookup"><span data-stu-id="9372f-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="9372f-110">若要深入瞭解，請參閱 [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)。</span><span class="sxs-lookup"><span data-stu-id="9372f-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
