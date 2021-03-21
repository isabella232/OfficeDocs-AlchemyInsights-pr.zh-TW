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
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>疑難排解 Azure AD 驗證和授權 (AADSTS) 錯誤碼

若要解決 AAD 驗證和授權錯誤碼 (AADSTS)，請執行下列建議步驟：

1. **處理應用程式中的錯誤碼**

- 此 **OAuth2.0 規格** https://tools.ietf.org/html/rfc6749#section-5.2 提供如何使用錯誤回應的錯誤部分，在驗證期間處理錯誤的指引。

    - **錯誤**： 錯誤碼字串，可用來分類發生的錯誤類型，而且應該用來回應錯誤。
    - **錯誤** 欄位有數個可能的值 - 請檢閱通訊協定文件連結和 OAuth 2.0 規格，以了解有關特定錯誤及如何回應錯誤的詳細資訊。

- 以下是範例錯誤回應：
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
2. **尋找目前的錯誤碼資訊**

- 錯誤碼和訊息可能會變更。 有關最新資訊，請參閱 https://login.microsoftonline.com/error 頁面，以尋找 AADSTS 的錯誤描述、修正，以及一些建議的因應措施。
- 您也可以搜尋並疑難排解列於文章 [Azure AD 驗證與授權錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application) (部分機器翻譯) 中的 [AADSTS 錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) (部分機器翻譯)。

3. **取得協助**

- [適用於開發人員的支援和協助選項](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) (部分機器翻譯) - 如果您需要問題解答，或協助解決我們文件中未涵蓋的問題，可以與專家連絡以取得協助。 本文提供數個在開發與 Microsoft 身分識別平台整合的應用程式時，取得問題的解答建議。








