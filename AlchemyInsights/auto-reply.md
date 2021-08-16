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
ms.openlocfilehash: 3ed937d38627c1089c9203550498ce7b21ce01c0c5a2deea7326f8057f5338d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036123"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>若要為所有傳送至 Microsoft 365 群組的電子郵件設定自動回覆:

**使用租用戶系統管理帳戶連接到 EXO PowerShell，並使用以下命令**:

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> 將 [groupmailbox]**** 變更為您想要在其上設定自動回覆的群組名稱。

