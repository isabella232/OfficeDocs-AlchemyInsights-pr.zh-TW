---
title: 連線至 MSCommerce 模組
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093536"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce 需要的公司或計費系統管理員帳戶

MSCommerce 模組需要有公司或計費系統管理員權限的帳戶。 如果您會收到下列錯誤，您必須使用不同的帳戶重新連線。

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

如果您的帳戶不具備公司或計費系統管理員權限，請連絡您的 IT 系統管理員。
