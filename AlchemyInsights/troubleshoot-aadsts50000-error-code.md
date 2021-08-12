---
title: 疑難排解 AADSTS50000 錯誤碼
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
- "9801"
- "9005744"
ms.openlocfilehash: 09c1a831c85ec6752c1df90b78d4a12158b4c9164b0cb388abf84fff745d35b3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939838"
---
# <a name="troubleshoot-aadsts50000-error-code"></a>疑難排解 AADSTS50000 錯誤碼

若要解決 AADSTS50000 錯誤，請執行下列步驟：

**AADSTS50000**：TokenIssuanceError - 登入服務有問題。

如果存取權杖要求有效且獲得授權，授權伺服器會簽發存取權杖和選擇性的重新整理權杖。 如果要求無法通過用戶端驗證或無效，授權伺服器會傳回錯誤回應。

授權伺服器會以錯誤碼回應，並且在回應中包含下列 **錯誤** 參數：

`invalid_request: The request is missing a required parameter, includes an unsupported parameter value (other than grant type), repeats a parameter, includes multiple credentials, utilizes more than one mechanism for authenticating the client, or is otherwise malformed.`

`invalid_client: Client authentication failed (e.g., unknown client, no client authentication included, or unsupported authentication method).  The authorization server MAY return an HTTP 401 (Unauthorized) status code to indicate which HTTP authentication schemes are supported.  If the client attempted to authenticate via the "Authorization" request header field, the authorization server MUST respond with an HTTP 401 (Unauthorized) status code and include the "WWW-Authenticate" response header field matching the authentication scheme used by the client.`

`invalid_grant: The provided authorization grant (e.g., authorization code, resource owner credentials) or refresh token is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client.`

`unauthorized_client: The authenticated client is not authorized to use this authorization grant type.`

`unsupported_grant_type: The authorization grant type is not supported by the authorization server.`

`invalid_scope: The requested scope is invalid, unknown, malformed, or exceeds the scope granted by the resource owner.`

[開啟支援票證](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-troubleshooting-support-howto)以解決此問題。