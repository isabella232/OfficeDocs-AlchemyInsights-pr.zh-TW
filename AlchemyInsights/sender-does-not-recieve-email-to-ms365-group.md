---
title: 寄件者不會收到傳送到 Microsoft 365 群組的電子郵件
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751306"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="f1a05-102">寄件者不會收到傳送到 Microsoft 365 群組的電子郵件</span><span class="sxs-lookup"><span data-stu-id="f1a05-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="f1a05-103">根據預設，將電子郵件訊息寄至 Microsoft 365 群組的寄件者不會在他們的收件匣中收到該郵件的複本，即使該寄件者是群組的成員。</span><span class="sxs-lookup"><span data-stu-id="f1a05-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="f1a05-104">使用此 EXO PowerShell 命令可讓寄件者能收到其傳送至 Microsoft 365 群組的每封電子郵件複本：</span><span class="sxs-lookup"><span data-stu-id="f1a05-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="f1a05-105">若要一次啟用所有信箱的設定：</span><span class="sxs-lookup"><span data-stu-id="f1a05-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="f1a05-106">**注意** 這項設定的變更需要 1 小時才會生效。</span><span class="sxs-lookup"><span data-stu-id="f1a05-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>