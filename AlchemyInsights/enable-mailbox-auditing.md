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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500273"
---
# <a name="enable-mailbox-auditing"></a>啟用信箱稽核

單一使用者或整個組織啟用信箱稽核必須從遠端 Power 命令介面執行下列 cmdlet：
  
 **單一使用者**
  
Set-mailbox-Identity"Jane Dow"-AuditEnabled $true
  
 **組織**
  
Get-mailbox ResultSize 不受限制-篩選 {RecipientTypeDetails-eq"UserMailbox"} |Set-mailbox AuditEnabled $true
  
[深入了解](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

