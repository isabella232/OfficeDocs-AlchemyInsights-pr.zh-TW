---
title: 修正 DKIM 記錄格式設定的常見問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736181"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="a4ea1-102">修正 DKIM 記錄格式設定的常見問題</span><span class="sxs-lookup"><span data-stu-id="a4ea1-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="a4ea1-103">大部分 DKIM 的設定問題與不正確的 DNS 記錄有關。</span><span class="sxs-lookup"><span data-stu-id="a4ea1-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="a4ea1-104">若要修正 DKIM 的設定問題，請確認 DKIM CNAME 記錄 (**不** 是 TXT 記錄) 的格式是否正確。</span><span class="sxs-lookup"><span data-stu-id="a4ea1-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="a4ea1-105">如需詳細資訊，請參閱 [在 Office 365 中手動設定 DKIM 所需執行](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)的動作。</span><span class="sxs-lookup"><span data-stu-id="a4ea1-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="a4ea1-106">如果您一般都需要 DNS 記錄的協助，請參閱 [在任何 dns 主機服務提供者處建立 dns 記錄，以進行 Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。</span><span class="sxs-lookup"><span data-stu-id="a4ea1-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="a4ea1-107">在您的網域的 DNS 主機服務上建立或更新 DKIM DNS 記錄之後，您必須等待 DNS 記錄傳播。</span><span class="sxs-lookup"><span data-stu-id="a4ea1-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
