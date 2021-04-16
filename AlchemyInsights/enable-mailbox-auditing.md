---
title: 啟用信箱稽核
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814183"
---
# <a name="enable-mailbox-auditing"></a>啟用信箱稽核

若要對單一使用者或整個組織啟用信箱審核，必須從遠端 Power Shell 執行下列 Cmdlet：
  
 **單一使用者**
  
Set-Mailbox 識別碼「Jane Dow」-AuditEnabled $true
  
 **組織**
  
Get-Mailbox ResultSize 無限制-篩選 {RecipientTypeDetails-eq "UserMailbox"} |Set-Mailbox-AuditEnabled $true
  
[深入了解](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

