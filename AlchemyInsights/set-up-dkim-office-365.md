---
title: 安裝 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808698"
---
# <a name="setup-dkim"></a>安裝 DKIM

在 Microsoft [365 的自](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)定義網域設定 DKIM 的完整指示如下。

1. 針對 **每個** 自訂網域，您必須在網域的 DNS 主機服務上建立 **兩個** DKIM CNAME 記錄：網域註冊機構)  (一般。 例如，contoso.com 和 fourthcoffee.com 需要四個 DKIM CNAME 記錄：兩個用於 contoso.com，而兩個用於 fourthcoffee.com。

   **每個**自訂網域的 DKIM CNAME 記錄使用下列格式：

   - **主機名稱**： `selector1._domainkey.<CustomDomain>`

     **指向 address 或 value**： `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**：3600

   - **主機名稱**： `selector2._domainkey.<CustomDomain>`

     **指向 address 或 value**： `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**：3600

   \<DomainGUID\> 是 `.mail.protection.outlook.com` 自訂網域之自訂 MX 記錄中的文字 (例如， `contoso-com` 針對 domain contoso.com) 。 \<InitialDomain\> 是您註冊 Microsoft 365 時所使用的網域 (例如，contoso.onmicrosoft.com) 。

2. 在您為自訂網域建立 CNAME 記錄後，請完成下列指示：

   a. 使用您的公司或學校帳戶登[入 Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) 。

   b. 選取左上角的應用程式啟動器圖示，然後選擇 [管理員]****。

   c. 在導覽的左下角展開 [管理員]****，然後選擇 [Exchange]****。

   d. 移至 [**保護**  >  **DKIM**]。

   e. 選取 [網域]，然後選擇 [**啟用****此網域的簽署郵件] 與 DKIM 的特徵碼**。 對每個自訂網域重複此步驟。
