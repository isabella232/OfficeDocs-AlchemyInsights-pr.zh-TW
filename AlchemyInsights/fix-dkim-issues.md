---
title: 修正 DKIM 安裝問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506765"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="8a7f8-102">修正 DKIM 安裝問題</span><span class="sxs-lookup"><span data-stu-id="8a7f8-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="8a7f8-103">如果您在為自訂網域啟用 DKIM 時遇到問題，請使用下列步驟：</span><span class="sxs-lookup"><span data-stu-id="8a7f8-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="8a7f8-104">大部分 DKIM 的設定問題都與不正確的 DNS 記錄有關。</span><span class="sxs-lookup"><span data-stu-id="8a7f8-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="8a7f8-105">確認 DKIM CNAME 記錄（**不**是 TXT 記錄）的格式設定正確。</span><span class="sxs-lookup"><span data-stu-id="8a7f8-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="8a7f8-106">如需詳細資訊，請參閱本[主題](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)。</span><span class="sxs-lookup"><span data-stu-id="8a7f8-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="8a7f8-107">在您的網域（通常是您的網域註冊機構）的 DNS 主機服務上建立或更新 DKIM DNS 記錄之後，請等候 DNS 記錄傳播。</span><span class="sxs-lookup"><span data-stu-id="8a7f8-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="8a7f8-108">如果您無法在系統管理中心建立 DKIM DNS 記錄，您可以取代您的 \<CustomDomain\> 自訂網域（例如，contoso.com），並在[Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行此命令 PowerShell： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 。</span><span class="sxs-lookup"><span data-stu-id="8a7f8-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
