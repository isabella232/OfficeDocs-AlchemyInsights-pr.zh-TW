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
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 3a7ffccadf6b415f7dd0d0871d368402332a0cd7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916731"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="90a47-102">啟用信箱稽核</span><span class="sxs-lookup"><span data-stu-id="90a47-102">Enable mailbox auditing</span></span>

<span data-ttu-id="90a47-103">單一使用者或整個組織啟用信箱稽核必須從遠端 Power 命令介面執行下列 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="90a47-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="90a47-104">**單一使用者**</span><span class="sxs-lookup"><span data-stu-id="90a47-104">**Single User**</span></span>
  
<span data-ttu-id="90a47-105">Set-mailbox-Identity"Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="90a47-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="90a47-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="90a47-106">**Organization**</span></span>
  
<span data-ttu-id="90a47-107">Get-mailbox ResultSize 不受限制-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="90a47-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="90a47-108">深入了解</span><span class="sxs-lookup"><span data-stu-id="90a47-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

