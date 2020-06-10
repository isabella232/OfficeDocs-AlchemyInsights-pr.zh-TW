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
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="5ec63-102">變更 Microsoft 365 群組的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="5ec63-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="5ec63-103">您可以使用系統管理中心來變更 Microsoft 365 群組的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="5ec63-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="5ec63-104">只要選取群組，然後選取 [@編輯電子郵件地址]。</span><span class="sxs-lookup"><span data-stu-id="5ec63-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="5ec63-105">您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組的主要 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="5ec63-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="5ec63-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="5ec63-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="5ec63-107">範例：</span><span class="sxs-lookup"><span data-stu-id="5ec63-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
