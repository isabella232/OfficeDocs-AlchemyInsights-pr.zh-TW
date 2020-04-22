---
title: 1374解析兩個信箱 howto
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 95d85d7737ae0684b2a2c017134104bd377695f1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722503"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="627eb-102">使用者有兩個信箱</span><span class="sxs-lookup"><span data-stu-id="627eb-102">A user has two mailboxes</span></span>

<span data-ttu-id="627eb-103">使用 Azure Active Directory Connect （AAD Connect）或 DirSync 的混合式環境可能會不小心導致使用者有兩個信箱：一個內部部署，另一個在雲端中。</span><span class="sxs-lookup"><span data-stu-id="627eb-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="627eb-104">在任何一個位置都可以建立重複的信箱。</span><span class="sxs-lookup"><span data-stu-id="627eb-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="627eb-105">若要解決此問題，請參閱 how [to 當信箱存在於 Exchange Online 和內部部署中時，如何復原](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises)。</span><span class="sxs-lookup"><span data-stu-id="627eb-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="627eb-106">如果您想要深入瞭解如何避免這種情況今後發生，請參閱我的[使用者在內部部署和 Exchange Online 中都有信箱。Help！](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809)。</span><span class="sxs-lookup"><span data-stu-id="627eb-106">If you want to learn more about how to avoid this from happening in the future, see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>
