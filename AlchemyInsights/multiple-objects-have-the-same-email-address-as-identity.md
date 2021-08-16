---
title: 多個物件的電子郵件地址與身份識別相同
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011903"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>多個物件的電子郵件地址與身份識別相同

**多個物件**

出現此錯誤的一個常見原因是，當多個物件的電子郵件地址與身分識別相同時，無法正確路由 Outlook Web Access 請求。若要尋找這些物件，請執行以下命令：

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