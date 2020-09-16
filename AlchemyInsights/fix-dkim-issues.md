---
title: 修正 DKIM 安裝問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744941"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="612be-102">修正 DKIM 安裝問題</span><span class="sxs-lookup"><span data-stu-id="612be-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="612be-103">如果您在為自訂網域啟用 DKIM 時遇到問題，請使用下列步驟：</span><span class="sxs-lookup"><span data-stu-id="612be-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="612be-104">大部分 DKIM 的設定問題都與不正確的 DNS 記錄有關。</span><span class="sxs-lookup"><span data-stu-id="612be-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="612be-105">驗證 DKIM CNAME 記錄 (**不** 是 TXT 記錄) 的格式是否正確。</span><span class="sxs-lookup"><span data-stu-id="612be-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="612be-106">如需詳細資訊，請參閱本 [主題](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)。</span><span class="sxs-lookup"><span data-stu-id="612be-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="612be-107">在您網域的 DNS 主機服務上建立或更新 DKIM DNS 記錄後，您的網域註冊機構) 中 (，請等候 DNS 記錄傳播。</span><span class="sxs-lookup"><span data-stu-id="612be-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="612be-108">如果您無法在系統管理中心建立 DKIM DNS 記錄，您可以取代您的 \<CustomDomain\> 自訂網域 (例如，contoso.com) 並在 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行此命令： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` 。</span><span class="sxs-lookup"><span data-stu-id="612be-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
