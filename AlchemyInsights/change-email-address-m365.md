---
title: 變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995613"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址

您可以使用 [Microsoft 365 系統管理中心](https://admin.microsoft.com/)來變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址。只要選取群組，然後選取 [@編輯電子郵件地址]。

您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組/Teams 的主要 SMTP 位址：

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

範例：

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
