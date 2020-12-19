---
title: 針對傳送至 Microsoft 365 群組的電子郵件收到的完整 NDR AggregateGroupMailbox
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715673"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="64a0b-102">針對傳送至 Microsoft 365 群組的電子郵件收到的完整 NDR AggregateGroupMailbox</span><span class="sxs-lookup"><span data-stu-id="64a0b-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="64a0b-103">使用下列 EXO 命令介面命令，建立 Exchange transport rule，以無訊息方式丟棄傳送至合計群組信箱的電子郵件：</span><span class="sxs-lookup"><span data-stu-id="64a0b-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="64a0b-104">使用您租使用者中的合計群組信箱的 SMTP 位址，取代 SMTP 位址 **SentTo** 。</span><span class="sxs-lookup"><span data-stu-id="64a0b-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="64a0b-105">您可以從收到的 NDR 取得合計群組信箱的 SMTP 位址。</span><span class="sxs-lookup"><span data-stu-id="64a0b-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



