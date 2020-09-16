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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733678"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="a5e84-102">變更 Microsoft 365 群組的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="a5e84-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="a5e84-103">您可以使用系統管理中心來變更 Microsoft 365 群組的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="a5e84-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="a5e84-104">只要選取群組，然後選取 [@編輯電子郵件地址]。</span><span class="sxs-lookup"><span data-stu-id="a5e84-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="a5e84-105">您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組的主要 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="a5e84-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="a5e84-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="a5e84-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="a5e84-107">範例：</span><span class="sxs-lookup"><span data-stu-id="a5e84-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
