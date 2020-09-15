---
title: 使用 Wix 網站搭配向 Microsoft 購買或受管理的網域
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: bef0943c8621043218088abf0deebddf6c19ef50
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664737"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="79298-102">使用 Wix 網站搭配向 Microsoft 購買或受管理的網域</span><span class="sxs-lookup"><span data-stu-id="79298-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="79298-103">如需如何使用 Wix 網站搭配向 Microsoft 購買或受管理的網域的相關資訊，請參閱[更新 DNS 記錄以便向目前的代管提供者保留網站](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)。</span><span class="sxs-lookup"><span data-stu-id="79298-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="79298-104">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="79298-104">For details, see:</span></span> 

- <span data-ttu-id="79298-105">Wix 文章「使用指向方法將網域連接至 Wix」(英文) 建議新增 DNS 記錄 (如以上連結中所概述)，而非在使用 Microsoft 365 時變更名稱伺服器。</span><span class="sxs-lookup"><span data-stu-id="79298-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="79298-106">如果您選擇將名稱伺服器變更為 Wix，則必須在 Wix 為 Microsoft 建立 DNS 記錄。</span><span class="sxs-lookup"><span data-stu-id="79298-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="79298-107">如需詳細資訊，請參閱[在 Wix 為 Microsoft 建立 DNS 記錄](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)。</span><span class="sxs-lookup"><span data-stu-id="79298-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="79298-108">如果您的網域是向 Microsoft 購買，則不能變更名稱伺服器。</span><span class="sxs-lookup"><span data-stu-id="79298-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="79298-109">如果您必須變更名稱伺服器，必須在 60天之後，將向 Microsoft 購買的網域轉移到另一個代管提供者。</span><span class="sxs-lookup"><span data-stu-id="79298-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="79298-110">如需詳細資訊，請參閱 [將網域從 Microsoft 傳送到另一個主機](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)。</span><span class="sxs-lookup"><span data-stu-id="79298-110">For more info, see [Transfer a domain from Microsoft to another host](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).</span></span>
