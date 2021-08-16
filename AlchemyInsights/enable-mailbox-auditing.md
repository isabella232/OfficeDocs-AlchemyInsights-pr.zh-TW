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
ms.openlocfilehash: 176fdc57c6453cafe6ca773d845f8f59ea782089e3e33ad70909ed495aa1a8c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003011"
---
# <a name="enable-mailbox-auditing"></a>啟用信箱稽核

若要對單一使用者或整個組織啟用信箱審核，必須從遠端 Power Shell 執行下列 Cmdlet：
  
 **單一使用者**
  
Set-Mailbox 識別碼「Jane Dow」-AuditEnabled $true
  
 **組織**
  
Get-Mailbox ResultSize 無限制-篩選 {RecipientTypeDetails-eq "UserMailbox"} |Set-Mailbox-AuditEnabled $true
  
[深入了解](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

