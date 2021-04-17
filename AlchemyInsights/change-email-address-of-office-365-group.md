---
title: 變更 Microsoft 365 群組的電子郵件地址
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819035"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="f5461-102">變更 Microsoft 365 群組的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="f5461-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="f5461-103">您可以使用系統管理中心來變更 Microsoft 365 群組的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="f5461-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="f5461-104">只要選取群組，然後選取 [@編輯電子郵件地址]。</span><span class="sxs-lookup"><span data-stu-id="f5461-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="f5461-105">您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組的主要 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="f5461-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="f5461-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="f5461-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="f5461-107">範例：</span><span class="sxs-lookup"><span data-stu-id="f5461-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
