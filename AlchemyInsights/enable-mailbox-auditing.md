---
title: 啟用信箱稽核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506945"
---
# <a name="enable-mailbox-auditing"></a>啟用信箱稽核

若要對單一使用者或整個組織啟用信箱審核，必須從遠端 Power Shell 執行下列 Cmdlet：
  
 **單一使用者**
  
Set-Mailbox 識別碼「Jane Dow」-AuditEnabled $true
  
 **組織**
  
Get-Mailbox ResultSize 無限制-篩選 {RecipientTypeDetails-eq "UserMailbox"} |Set-Mailbox-AuditEnabled $true
  
[深入了解](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

