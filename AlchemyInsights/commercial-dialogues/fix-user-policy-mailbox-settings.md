---
title: 修正使用者原則/信箱設定
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736150"
---
# <a name="fix-user-policymailbox-settings"></a>修正使用者原則/信箱設定

信箱上的垃圾郵件設定會影響此郵件。 若要複查設定，請執行下列操作：

1. 啟動 Exchange 管理命令介面。 如需詳細資訊，請參閱 [開啟 Exchange 管理命令](https://go.microsoft.com/fwlink/?linkid=2101432)介面。
2. 使用使用者的電子郵件地址執行此命令 () ：  **mailboxjunkmailconfiguration-identity "user@domain.com"**
3. 檢查寄件者的電子郵件地址是否屬於 **TrustedSendersAndDomains** 或 **BlockedSendersAndDomains**。 如果電子郵件地址位於其中一個清單中，您可能必須加以移除。 若要深入瞭解，請參閱 [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)。
