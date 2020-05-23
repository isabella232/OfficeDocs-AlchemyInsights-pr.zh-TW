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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282253"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="c57f3-102">變更 Microsoft 365 群組的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="c57f3-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="c57f3-103">您可以使用系統管理中心來變更 Microsoft 365 群組的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="c57f3-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c57f3-104">只要選取群組，然後選取 [@編輯電子郵件地址]。</span><span class="sxs-lookup"><span data-stu-id="c57f3-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c57f3-105">您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組的主要 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="c57f3-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="c57f3-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c57f3-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c57f3-107">範例：</span><span class="sxs-lookup"><span data-stu-id="c57f3-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
