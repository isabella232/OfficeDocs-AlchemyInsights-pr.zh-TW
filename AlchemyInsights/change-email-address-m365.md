---
title: 變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756548"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="1c769-102">變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="1c769-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="1c769-103">您可以使用 [Microsoft 365 系統管理中心](https://admin.microsoft.com/)來變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="1c769-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="1c769-104">只要選取群組，然後選取 [@編輯電子郵件地址]。</span><span class="sxs-lookup"><span data-stu-id="1c769-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="1c769-105">您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組/Teams 的主要 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="1c769-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="1c769-106">範例：</span><span class="sxs-lookup"><span data-stu-id="1c769-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
