---
title: 安裝 Office 365 中的 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666255"
---
# <a name="setup-dkim-in-office-365"></a>安裝 Office 365 中的 DKIM

為 Office 365 中的自訂網域設定 DKIM 的完整指示[以下](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)。

1. **每**個自訂網域，您需要建立**兩個**DKIM 筆 CNAME 記錄在您的網域 DNS 主機服務 （通常是網域註冊機構）。 例如，contoso.com 及 fourthcoffee.com 需要四個 DKIM CNAME 記錄： contoso.com 及 fourthcoffee.com 的兩個。

   **每個**自訂網域的 DKIM CNAME 記錄使用下列格式：

   - **主機名稱**：`selector1._domainkey.<CustomDomain>`

     **指向位址] 或 [值**：`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **主機名稱**：`selector2._domainkey.<CustomDomain>`

     **指向位址] 或 [值**：`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>是左邊的文字`.mail.protection.outlook.com`中自訂 MX 記錄中的自訂網域 (例如，`contoso-com`網域 contoso.com)。 \<InitialDomain\>是您的 Office 365 (例如，contoso.onmicrosoft.com) 的註冊時所用的網域。

2. 您已建立的 CNAME 記錄為您自訂的網域之後，請完成下列指示：

   a. 使用您的 公司或學校帳戶[登入 Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)。

   b. 選取左上角的應用程式啟動器圖示，然後選擇 [管理員]****。

   c. 左下導覽中，依序展開 [**系統管理員**，並選擇 [ **Exchange**]。

   d. 移至 [**保護** > **DKIM**。

   e. 選取 [網域]，然後選擇**此網域的 DKIM 簽章簽署**郵件的 [**啟用**。 針對每個自訂網域重複此步驟。
