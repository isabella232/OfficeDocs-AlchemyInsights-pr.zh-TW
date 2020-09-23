---
title: 726封鎖電子郵件轉發
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219846"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>封鎖或取消封鎖電子郵件轉發

若要啟用或停用特定信箱的電子郵件轉寄功能，請參閱 [設定電子郵件轉接](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。

在租使用者層級上，使用輸出反垃圾郵件原則來控制外部轉寄。 若設為 [關閉] 或 [自動]，它可能會封鎖「550 5.7.520 存取權遭到拒絕，您的組織不允許外部轉送」的電子郵件轉寄錯誤。 接著，如果轉寄設定為封鎖，就表示您的使用者會看到錯誤。

如果已封鎖轉接，請確定原則已設定為啟用外部 Autoforward。 您可以從安全性與合規性中心或執行命令 Get-HostedOutboundSpamFilterPolicy，檢查輸出垃圾郵件篩選原則。fl 名稱，AutoForwardingMode。 如果您想要設定 Autoforward 封鎖，相同的命令會立即告知您的原則狀態。

附注：建議您在預設的輸出垃圾郵件篩選原則上停用外部 Autoforward，並僅針對需要外部轉寄的使用者，為這些使用者建立自訂原則加以啟用。 您可以在 Office 365 中深入瞭解設定 [外部電子郵件](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)轉寄。