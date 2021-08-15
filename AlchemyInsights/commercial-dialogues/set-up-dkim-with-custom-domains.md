---
title: 使用自訂網域設定 DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994783"
---
# <a name="set-up-dkim-with-custom-domains"></a>使用自訂網域設定 DKIM

您必須為 DNS 中的每個自訂網域發佈兩筆 CNAME 記錄。 若要這麼做，請使用下列格式：

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** 是自訂網域之自訂 MX 記錄中的 **mail.protection.outlook.com** 左邊的文字 (例如，contoso-com for domain **contoso.com**) 。 **InitialDomain** 是您註冊 Office 365 時所使用的網域 (例如， **contoso.onmicrosoft.com**) 。

如需 DNS 記錄的詳細資訊，請參閱[在任何 DNS 主機服務提供者處建立 dns 記錄以進行 Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。