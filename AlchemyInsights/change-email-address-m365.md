---
title: 變更 Microsoft 365 群組的電子郵件地址
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416691"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>變更一個 Microsoft 365 群組的電子郵件地址

您可以使用系統管理中心來變更 Microsoft 365 群組的電子郵件地址。 只要選取群組，然後選取 [@編輯電子郵件地址]。

您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組的主要 SMTP 位址：

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

範例：

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
