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
ms.openlocfilehash: 1ef60017f1ea656296bc7b2aa3bc5365646f11f3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527587"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="7a008-102">啟用信箱稽核</span><span class="sxs-lookup"><span data-stu-id="7a008-102">Enable mailbox auditing</span></span>

<span data-ttu-id="7a008-103">若要啟用單一使用者或整個組織的信箱稽核，必須從 Power 的遠端命令介面執行下列 cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7a008-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="7a008-104">**單一使用者**</span><span class="sxs-lookup"><span data-stu-id="7a008-104">**Single User**</span></span>
  
<span data-ttu-id="7a008-105">Set-mailbox-Identity"Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7a008-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="7a008-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="7a008-106">**Organization**</span></span>
  
<span data-ttu-id="7a008-107">Get-mailbox ResultSize Unlimited-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="7a008-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="7a008-108">深入了解</span><span class="sxs-lookup"><span data-stu-id="7a008-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

