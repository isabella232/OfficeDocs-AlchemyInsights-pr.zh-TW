---
title: 搜尋並刪除組織中的電子郵件
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948874"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>搜尋並刪除組織中的電子郵件

請遵循下列步驟：

1. 若您不是全域系統管理員，若要搜尋郵件，您的帳戶必須新增至 **EDiscovery 管理員角色群組** 或 **符合性搜尋管理角色**。 若要刪除郵件，您需要加入「 **組織管理」角色群組** 或「 **搜尋並清除」管理角色**。 在[安全性 & 規範中心](https://protection.office.com)指派這些角色的許可權。
2. [建立內容搜尋](https://docs.microsoft.com/office365/securitycompliance/content-search) ，以尋找要刪除的郵件。
3. [連線到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。 如果您使用的是 MFA，請參閱下列指示：[使用多重要素驗證連線到安全性 & 規範中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. 刪除郵件：執行 `New-ComplianceSearchAction` Cmdlet 以刪除郵件。 已刪除的郵件會移至使用者的 [可復原的項目] 資料夾。 如需範例命令，請參閱 [Step 3： Delete the message。](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
