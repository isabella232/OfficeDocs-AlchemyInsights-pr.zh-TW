---
title: 疑難排解 Azure AD 驗證和授權 (AADSTS) 錯誤碼
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
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897834"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="90be8-102">疑難排解 Azure AD 驗證和授權 (AADSTS) 錯誤碼</span><span class="sxs-lookup"><span data-stu-id="90be8-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="90be8-103">若要解決 AAD 驗證和授權錯誤碼 (AADSTS)，請執行下列建議步驟：</span><span class="sxs-lookup"><span data-stu-id="90be8-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="90be8-104">**處理應用程式中的錯誤碼**</span><span class="sxs-lookup"><span data-stu-id="90be8-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="90be8-105">此 **OAuth2.0 規格** https://tools.ietf.org/html/rfc6749#section-5.2 提供如何使用錯誤回應的錯誤部分，在驗證期間處理錯誤的指引。</span><span class="sxs-lookup"><span data-stu-id="90be8-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="90be8-106">**錯誤**： 錯誤碼字串，可用來分類發生的錯誤類型，而且應該用來回應錯誤。</span><span class="sxs-lookup"><span data-stu-id="90be8-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="90be8-107">**錯誤** 欄位有數個可能的值 - 請檢閱通訊協定文件連結和 OAuth 2.0 規格，以了解有關特定錯誤及如何回應錯誤的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="90be8-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="90be8-108">以下是範例錯誤回應：</span><span class="sxs-lookup"><span data-stu-id="90be8-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="90be8-109">**尋找目前的錯誤碼資訊**</span><span class="sxs-lookup"><span data-stu-id="90be8-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="90be8-110">錯誤碼和訊息可能會變更。</span><span class="sxs-lookup"><span data-stu-id="90be8-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="90be8-111">有關最新資訊，請參閱 https://login.microsoftonline.com/error 頁面，以尋找 AADSTS 的錯誤描述、修正，以及一些建議的因應措施。</span><span class="sxs-lookup"><span data-stu-id="90be8-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="90be8-112">您也可以搜尋並疑難排解列於文章 [Azure AD 驗證與授權錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application) (部分機器翻譯) 中的 [AADSTS 錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="90be8-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="90be8-113">**取得協助**</span><span class="sxs-lookup"><span data-stu-id="90be8-113">**Get Help**</span></span>

- <span data-ttu-id="90be8-114">[適用於開發人員的支援和協助選項](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) (部分機器翻譯) - 如果您需要問題解答，或協助解決我們文件中未涵蓋的問題，可以與專家連絡以取得協助。</span><span class="sxs-lookup"><span data-stu-id="90be8-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="90be8-115">本文提供數個在開發與 Microsoft 身分識別平台整合的應用程式時，取得問題的解答建議。</span><span class="sxs-lookup"><span data-stu-id="90be8-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>








