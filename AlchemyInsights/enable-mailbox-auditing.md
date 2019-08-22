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
# <a name="enable-mailbox-auditing"></a>啟用信箱稽核

若要啟用單一使用者或整個組織的信箱稽核，必須從 Power 的遠端命令介面執行下列 cmdlet:
  
 **單一使用者**
  
Set-mailbox-Identity"Jane Dow"-AuditEnabled $true
  
 **組織**
  
Get-mailbox ResultSize Unlimited-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox-AuditEnabled $true
  
[深入了解](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

