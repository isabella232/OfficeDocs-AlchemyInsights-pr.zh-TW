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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034709"
---
# <a name="fix-user-policymailbox-settings"></a>修正使用者原則/信箱設定

信箱上的垃圾郵件設定會影響此郵件。 若要複查設定，請執行下列操作：

1. 啟動 Exchange 管理命令介面。 如需詳細資訊，請參閱[Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432)。
2. 使用使用者的電子郵件地址執行此命令 () ：  **mailboxjunkmailconfiguration-identity "user@domain.com"**
3. 檢查寄件者的電子郵件地址是否屬於 **TrustedSendersAndDomains** 或 **BlockedSendersAndDomains**。 如果電子郵件地址位於其中一個清單中，您可能必須加以移除。 若要深入瞭解，請參閱 [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)。
