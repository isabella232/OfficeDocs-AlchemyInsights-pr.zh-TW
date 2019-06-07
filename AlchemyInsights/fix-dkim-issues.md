---
title: 解決 DKIM 設定問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764889"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="76160-102">解決 DKIM 設定問題</span><span class="sxs-lookup"><span data-stu-id="76160-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="76160-103">如果您遇到問題的自訂網域啟用 DKIM，請使用下列步驟：</span><span class="sxs-lookup"><span data-stu-id="76160-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="76160-104">不正確的 DNS 記錄相關大部分 DKIM 設定問題。</span><span class="sxs-lookup"><span data-stu-id="76160-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="76160-105">確認正確地格式化 DKIM CNAME 記錄 （\*\*\*\* TXT 記錄）。</span><span class="sxs-lookup"><span data-stu-id="76160-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="76160-106">如需詳細資訊，請參閱本[主題](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)。</span><span class="sxs-lookup"><span data-stu-id="76160-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="76160-107">之後您建立或更新您的 DKIM DNS 記錄，在 DNS 裝載服務，您的網域 （通常是您的網域註冊機構），等候 DNS 記錄，才能傳播。</span><span class="sxs-lookup"><span data-stu-id="76160-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="76160-108">如果您不能在系統管理中心建立 DKIM DNS 記錄，您可以取代\<CustomDomain\>與您的自訂網域 (例如，contoso.com) 和[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行此命令： `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`。</span><span class="sxs-lookup"><span data-stu-id="76160-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
