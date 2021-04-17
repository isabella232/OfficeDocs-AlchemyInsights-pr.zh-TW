---
title: 解決 SMTP 驗證問題
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826406"
---
# <a name="solving-smtp-authentication-issues"></a>解決 SMTP 驗證問題

如果您在嘗試傳送 SMTP 電子郵件，並在使用用戶端或應用程式進行驗證時收到錯誤 5.7.57 或 5.7.3，您應檢查下列事項：

- 在您的租用戶中或您嘗試使用的信箱上 (檢查這兩項設定)，已驗證的 SMTP 提交可能已停用。 若要閱讀更多相關資訊，請參閱[啟用或停用已驗證用戶端 SMTP 提交](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission) \(部分機器翻譯\)。

- 檢查是否為您的租用戶啟用 [Azure 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) \(部分機器翻譯\)；如果啟用，使用基本驗證 (也稱為舊版驗證，這會使用使用者名稱和密碼) 的 SMTP 驗證將會失敗。
