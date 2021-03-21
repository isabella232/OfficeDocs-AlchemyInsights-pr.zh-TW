---
title: 疑難排解錯誤碼 AADSTS50011
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901609"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="70789-102">疑難排解錯誤碼 AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="70789-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="70789-103">若要解決 AADSTS50011 錯誤，請執行下列建議步驟。</span><span class="sxs-lookup"><span data-stu-id="70789-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="70789-104">**AADSTS50011**：InvalidReplyTo - 回覆地址遺失、設定錯誤或不符合為應用程式所設定的回覆地址。</span><span class="sxs-lookup"><span data-stu-id="70789-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="70789-105">解決方案是確保將此遺失的回覆地址新增到 Azure Active Directory (AD) 應用程式，或請具有權限在 AD 中管理您的應用程式的人員，為您執行此操作。</span><span class="sxs-lookup"><span data-stu-id="70789-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="70789-106">如需詳細資訊，請參閱錯誤 [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch) 的疑難排解文章。</span><span class="sxs-lookup"><span data-stu-id="70789-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>