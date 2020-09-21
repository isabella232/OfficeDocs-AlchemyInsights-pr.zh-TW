---
title: 解決 SMTP 驗證問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737980"
---
# <a name="solving-smtp-authentication-issues"></a>解決 SMTP 驗證問題

如果您在嘗試傳送 SMTP 電子郵件，並在使用用戶端或應用程式進行驗證時收到錯誤 5.7.57 或 5.7.3，您應檢查下列事項：

- 在您的租用戶中或您嘗試使用的信箱上 (檢查這兩項設定)，已驗證的 SMTP 提交可能已停用。 若要閱讀更多相關資訊，請參閱[啟用或停用已驗證用戶端 SMTP 提交](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission) \(部分機器翻譯\)。

- 檢查是否為您的租用戶啟用 [Azure 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) \(部分機器翻譯\)；如果啟用，使用基本驗證 (也稱為舊版驗證，這會使用使用者名稱和密碼) 的 SMTP 驗證將會失敗。
