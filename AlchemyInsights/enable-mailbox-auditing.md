---
title: 啟用信箱稽核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806282"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="59c61-102">啟用信箱稽核</span><span class="sxs-lookup"><span data-stu-id="59c61-102">Enable mailbox auditing</span></span>

<span data-ttu-id="59c61-103">若要對單一使用者或整個組織啟用信箱審核，必須從遠端 Power Shell 執行下列 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="59c61-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="59c61-104">**單一使用者**</span><span class="sxs-lookup"><span data-stu-id="59c61-104">**Single User**</span></span>
  
<span data-ttu-id="59c61-105">Set-Mailbox 識別碼「Jane Dow」-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="59c61-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="59c61-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="59c61-106">**Organization**</span></span>
  
<span data-ttu-id="59c61-107">Get-Mailbox ResultSize 無限制-篩選 {RecipientTypeDetails-eq "UserMailbox"} |Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="59c61-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="59c61-108">深入了解</span><span class="sxs-lookup"><span data-stu-id="59c61-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

