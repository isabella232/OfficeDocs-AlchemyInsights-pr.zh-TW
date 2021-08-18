---
title: 針對傳送至 Microsoft 365 群組的電子郵件收到完整 NDR AggregateGroupMailbox
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315901"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>針對傳送至 Microsoft 365 群組的電子郵件收到完整 NDR AggregateGroupMailbox

使用下列 EXO 命令介面命令，建立 Exchange 傳輸規則，以無訊息方式投遞傳送至合計群組信箱的電子郵件：

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**附注**：使用您租使用者中的合計群組信箱的 smtp 位址，取代 smtp 位址 **SentTo** 。 您可以從收到的 NDR 取得合計群組信箱的 SMTP 位址。



