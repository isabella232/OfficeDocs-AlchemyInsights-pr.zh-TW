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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059623"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>封鎖或取消封鎖電子郵件轉發

若要啟用或停用特定信箱的電子郵件轉寄功能，請參閱 [設定電子郵件轉接](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。

在租使用者層級上，會使用輸出垃圾郵件原則來控制外部轉送。 您可以從 [這裡](https://protection.office.com/antispam) 的安全性與合規性中心檢查輸出垃圾郵件篩選原則，或使用 [Get-HostedOutboundSpamFilterPolicy 命令](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)。

如果您收到下列錯誤：「 **550 5.7.520 存取權遭到拒絕，您的組織不允許外部轉送**」，請確定原則已設定為啟用外部自動轉寄。

**附注：** 建議您在預設的輸出垃圾郵件篩選原則上停用外部 Autoforward，並僅針對需要外部轉寄的使用者，為這些使用者建立自訂原則加以啟用。 您可以在 Office 365 中深入瞭解設定[外部電子郵件轉發](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。