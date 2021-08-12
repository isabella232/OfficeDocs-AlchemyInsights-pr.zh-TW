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
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958288"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>寄件者不會收到傳送到 Microsoft 365 群組的電子郵件

根據預設，將電子郵件訊息寄至 Microsoft 365 群組的寄件者不會在他們的收件匣中收到該郵件的複本，即使該寄件者是群組的成員。

使用此 EXO PowerShell 命令可讓寄件者能收到其傳送至 Microsoft 365 群組的每封電子郵件複本：  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

若要一次啟用所有信箱的設定：

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**注意** 這項設定的變更需要 1 小時才會生效。