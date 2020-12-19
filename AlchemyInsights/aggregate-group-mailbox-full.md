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
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>針對傳送至 Microsoft 365 群組的電子郵件收到的完整 NDR AggregateGroupMailbox

使用下列 EXO 命令介面命令，建立 Exchange transport rule，以無訊息方式丟棄傳送至合計群組信箱的電子郵件：

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> 使用您租使用者中的合計群組信箱的 SMTP 位址，取代 SMTP 位址 **SentTo** 。 您可以從收到的 NDR 取得合計群組信箱的 SMTP 位址。



