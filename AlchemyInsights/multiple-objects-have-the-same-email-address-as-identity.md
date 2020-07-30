---
title: 多個物件的電子郵件地址與身份識別相同
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431340"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>多個物件的電子郵件地址與身份識別相同

**多個物件**

出現此錯誤的一個常見原因是，當多個物件的電子郵件地址與身份識別相同時，無法正確路由 Outlook Web Access 請求。 要尋找這些物件，請運行以下命令：

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

若要解決此問題，請删除具有相同電子郵件識別的多個物件，並確保存在一個具有特定電子郵件識別的物件，並且其收件者類型為 UserMailbox。

**商務和消費者信箱使用同一地址**

另一個原因是，商務和消費者信箱使用相同的位址。 在此情況下，使用者必須變更其主要消費者別名，直到咖啡廳支援此案例。 這是永久性錯誤，沒有干預就不能消失。

如需詳細資訊，請參閱[變更您 Microsoft 帳戶的電子郵件地址或電話號碼](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)。