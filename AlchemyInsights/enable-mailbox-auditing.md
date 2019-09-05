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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736244"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="9dd92-102">啟用信箱稽核</span><span class="sxs-lookup"><span data-stu-id="9dd92-102">Enable mailbox auditing</span></span>

<span data-ttu-id="9dd92-103">若要啟用單一使用者或整個組織的信箱稽核，必須從 Power 的遠端命令介面執行下列 cmdlet:</span><span class="sxs-lookup"><span data-stu-id="9dd92-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="9dd92-104">**單一使用者**</span><span class="sxs-lookup"><span data-stu-id="9dd92-104">**Single User**</span></span>
  
<span data-ttu-id="9dd92-105">Set-mailbox-Identity"Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="9dd92-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="9dd92-106">**組織**</span><span class="sxs-lookup"><span data-stu-id="9dd92-106">**Organization**</span></span>
  
<span data-ttu-id="9dd92-107">Get-mailbox ResultSize Unlimited-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="9dd92-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="9dd92-108">深入了解</span><span class="sxs-lookup"><span data-stu-id="9dd92-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

