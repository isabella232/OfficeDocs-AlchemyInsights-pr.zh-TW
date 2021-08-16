---
title: 開啟信箱審計
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058029"
---
# <a name="turn-on-mailbox-auditing"></a>開啟信箱審計

若要開啟單一使用者或整個組織的信箱審核，請從遠端 PowerShell: 執行下列 Cmdlet

- **單一使用者**： Set-Mailbox 身分識別「Jane Dow」-AuditEnabled $true
- **組織**： Get-Mailbox ResultSize 無限制-篩選器 {RecipientTypeDetails-eq "UserMailbox"} |Set-Mailbox-AuditEnabled $true

若要深入瞭解，請參閱 [管理信箱審核](https://go.microsoft.com/fwlink/?linkid=2103668)。