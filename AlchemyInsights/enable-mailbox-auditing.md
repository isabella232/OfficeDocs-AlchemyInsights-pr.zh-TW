---
title: 啟用信箱稽核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403738"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="df30c-102">啟用信箱稽核</span><span class="sxs-lookup"><span data-stu-id="df30c-102">Enable mailbox auditing</span></span>

<span data-ttu-id="df30c-103">若要啟用單一使用者或整個組織的信箱稽核，必須從 Power 的遠端命令介面執行下列 cmdlet:</span><span class="sxs-lookup"><span data-stu-id="df30c-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="df30c-104">**單一使用者**</span><span class="sxs-lookup"><span data-stu-id="df30c-104">**Single User**</span></span>
  
<span data-ttu-id="df30c-105">Set-mailbox-Identity"Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="df30c-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="df30c-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="df30c-106">**Organization**</span></span>
  
<span data-ttu-id="df30c-107">Get-mailbox ResultSize Unlimited-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="df30c-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="df30c-108">深入了解</span><span class="sxs-lookup"><span data-stu-id="df30c-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

