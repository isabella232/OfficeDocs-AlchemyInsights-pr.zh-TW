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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735797"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="81e7f-102">使用自訂網域設定 DKIM</span><span class="sxs-lookup"><span data-stu-id="81e7f-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="81e7f-103">您必須為 DNS 中的每個自訂網域發佈兩筆 CNAME 記錄。</span><span class="sxs-lookup"><span data-stu-id="81e7f-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="81e7f-104">若要這麼做，請使用下列格式：</span><span class="sxs-lookup"><span data-stu-id="81e7f-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="81e7f-105">**DomainGUID** 是自訂網域之自訂 MX 記錄中的 **mail.protection.outlook.com** 左邊的文字 (例如，contoso-com for domain **contoso.com**) 。</span><span class="sxs-lookup"><span data-stu-id="81e7f-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="81e7f-106">**InitialDomain** 是您註冊 Office 365 (時所使用的網域，例如， **contoso.onmicrosoft.com**) 。</span><span class="sxs-lookup"><span data-stu-id="81e7f-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="81e7f-107">如需 DNS 記錄的詳細資訊，請參閱 [在 Office 365 的任何 DNS 主機服務提供者中建立 dns 記錄](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。</span><span class="sxs-lookup"><span data-stu-id="81e7f-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>