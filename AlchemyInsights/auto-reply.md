---
title: '若要為所有傳送至 Microsoft 365 群組的電子郵件設定自動回覆:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331522"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>若要為所有傳送至 Microsoft 365 群組的電子郵件設定自動回覆:

**使用租用戶系統管理帳戶連接到 EXO PowerShell，並使用以下命令**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**注意**：將 **[groupmailbox]** 變更為您想要在其上設定自動回覆的群組名稱。

