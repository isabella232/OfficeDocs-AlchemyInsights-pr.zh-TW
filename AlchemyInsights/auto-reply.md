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
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430720"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a><span data-ttu-id="15547-102">若要為所有傳送至 Microsoft 365 群組的電子郵件設定自動回覆:</span><span class="sxs-lookup"><span data-stu-id="15547-102">To configure auto reply for all emails sent to Microsoft 365 group:</span></span>

<span data-ttu-id="15547-103">**使用租用戶系統管理帳戶連接到 EXO PowerShell，並使用以下命令**:</span><span class="sxs-lookup"><span data-stu-id="15547-103">**Connect to EXO PowerShell using tenant admin account and use following command**:</span></span>

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> <span data-ttu-id="15547-104">將 [groupmailbox]\*\*\*\* 變更為您想要在其上設定自動回覆的群組名稱。</span><span class="sxs-lookup"><span data-stu-id="15547-104">Change **groupmailbox** to a group name that you want to configure auto reply on.</span></span>

