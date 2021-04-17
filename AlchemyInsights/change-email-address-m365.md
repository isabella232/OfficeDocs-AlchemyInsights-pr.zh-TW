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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819071"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="9ff39-102">變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="9ff39-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="9ff39-103">您可以使用 [Microsoft 365 系統管理中心](https://admin.microsoft.com/)來變更 Microsoft 365 群組或 Microsoft Teams 的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="9ff39-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="9ff39-104">只要選取群組，然後選取 [@編輯電子郵件地址]。</span><span class="sxs-lookup"><span data-stu-id="9ff39-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="9ff39-105">您也可以使用下列 EXO PowerShell 命令來變更 Microsoft 365 群組/Teams 的主要 SMTP 位址：</span><span class="sxs-lookup"><span data-stu-id="9ff39-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="9ff39-106">範例：</span><span class="sxs-lookup"><span data-stu-id="9ff39-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
