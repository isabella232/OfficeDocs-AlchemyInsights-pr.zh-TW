---
title: 變更 Microsoft 365 群組的電子郵件地址
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580648"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>變更 Microsoft 365 群組的電子郵件地址

您可以使用系統管理中心來變更 Microsoft 365 群組的電子郵件地址。 只要選取群組，然後選取 [@編輯電子郵件地址]。

您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組的主要 SMTP 位址：

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

範例：

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
