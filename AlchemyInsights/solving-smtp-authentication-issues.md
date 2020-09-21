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
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="3ba77-102">解決 SMTP 驗證問題</span><span class="sxs-lookup"><span data-stu-id="3ba77-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="3ba77-103">如果您在嘗試傳送 SMTP 電子郵件，並在使用用戶端或應用程式進行驗證時收到錯誤 5.7.57 或 5.7.3，您應檢查下列事項：</span><span class="sxs-lookup"><span data-stu-id="3ba77-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="3ba77-104">在您的租用戶中或您嘗試使用的信箱上 (檢查這兩項設定)，已驗證的 SMTP 提交可能已停用。</span><span class="sxs-lookup"><span data-stu-id="3ba77-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="3ba77-105">若要閱讀更多相關資訊，請參閱[啟用或停用已驗證用戶端 SMTP 提交](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission) \(部分機器翻譯\)。</span><span class="sxs-lookup"><span data-stu-id="3ba77-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="3ba77-106">檢查是否為您的租用戶啟用 [Azure 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) \(部分機器翻譯\)；如果啟用，使用基本驗證 (也稱為舊版驗證，這會使用使用者名稱和密碼) 的 SMTP 驗證將會失敗。</span><span class="sxs-lookup"><span data-stu-id="3ba77-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
