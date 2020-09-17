---
title: 錯誤碼 550 5.7.501 存取遭到拒絕，偵測到垃圾郵件濫用
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784046"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="cb339-102">550 5.7.501 存取遭到拒絕，偵測到垃圾郵件濫用</span><span class="sxs-lookup"><span data-stu-id="cb339-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="cb339-103">一般來說，當使用者使用指派給 Microsoft 365 中新租使用者的 *onmicrosoft.com* 網域從 IP 位址傳送電子郵件時，就會發生此訊息。</span><span class="sxs-lookup"><span data-stu-id="cb339-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="cb339-104">若要解決此問題，最簡單的方法是：</span><span class="sxs-lookup"><span data-stu-id="cb339-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="cb339-105">[將網域新增至您的租使用者](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)。</span><span class="sxs-lookup"><span data-stu-id="cb339-105">[Add a domain to your tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="cb339-106">[將使用者的主要電子郵件地址變更](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) 為您剛新增的新自訂網域。</span><span class="sxs-lookup"><span data-stu-id="cb339-106">[Change your users' primary email address](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
