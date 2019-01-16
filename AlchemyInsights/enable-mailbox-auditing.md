---
title: 啟用信箱稽核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278217"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="bb34d-102">啟用信箱稽核</span><span class="sxs-lookup"><span data-stu-id="bb34d-102">Enable mailbox auditing</span></span>

<span data-ttu-id="bb34d-103">單一使用者或整個組織啟用信箱稽核必須從遠端 Power 命令介面執行下列 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="bb34d-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="bb34d-104">**單一使用者**</span><span class="sxs-lookup"><span data-stu-id="bb34d-104">**Single User**</span></span>
  
<span data-ttu-id="bb34d-105">Set-mailbox-Identity"Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bb34d-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="bb34d-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="bb34d-106">**Organization**</span></span>
  
<span data-ttu-id="bb34d-107">Get-mailbox ResultSize 不受限制-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="bb34d-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="bb34d-108">深入了解</span><span class="sxs-lookup"><span data-stu-id="bb34d-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

