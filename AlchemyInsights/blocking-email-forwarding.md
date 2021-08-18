---
title: 封鎖或解除封鎖外部自動電子郵件轉接
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315865"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>封鎖或解除封鎖外部自動電子郵件轉接

若要啟用或停用特定信箱的電子郵件轉寄功能，請參閱 [設定電子郵件轉接](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。

系統管理員可以使用 [輸出垃圾郵件原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)來控制組織的外部轉送。 您可以在 Microsoft 365 Defender 入口網站中管理輸出垃圾郵件原則， <https://security.microsoft.com/antispam> 也可以使用 Exchange Online PowerShell 中的[Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Cmdlet 來管理。

如果您收到下列錯誤：「 **550 5.7.520 存取權遭到拒絕，您的組織不允許外部轉送**」，請確定原則已設定為啟用外部自動轉寄的郵件。

**附注**：建議您在預設輸出垃圾郵件篩選原則中，自動轉寄 **規則** 的預設值 **受管理** 的預設值會封鎖預設的輸出垃圾郵件篩選原則 (會封鎖自動外部轉送;內部自動轉寄仍可運作) 。 您應建立自訂輸出垃圾郵件篩選原則，並使用轉寄值僅針對需要外部自動電子郵件轉寄的使用者 **啟用** 。 如需詳細資訊，請參閱[在 Office 365 中設定外部電子郵件轉發](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。
