---
title: 使用 AAD 網域服務的虛擬組態
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884564"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="ce12f-102">使用 AAD 網域服務的虛擬組態</span><span class="sxs-lookup"><span data-stu-id="ce12f-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="ce12f-103">使用 AAD 網域服務的虛擬組態涉及下列步驟：</span><span class="sxs-lookup"><span data-stu-id="ce12f-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="ce12f-104">正在檢查 [Microsoft Azure 入口網站] 上您的網域健康情況 https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="ce12f-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="ce12f-105">正在檢查您的 NSG 是否有針對入口網站上的 Azure AD Domain Services 同步處理的連接埠進行封鎖的規則 https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="ce12f-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="ce12f-106">確保您的虛擬網路部署在與管理 Azure AD Domain Services 網域相同的 Azure 區域。</span><span class="sxs-lookup"><span data-stu-id="ce12f-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="ce12f-107">確保您擁有的現有網域名稱並未與虛擬網路使用的網域名稱相同。</span><span class="sxs-lookup"><span data-stu-id="ce12f-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="ce12f-108">如需有關 Azure 虛擬網路與支援 AAD 網域服務的 的設計考量詳細資訊，請參閱 [虛擬網路考量](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)。</span><span class="sxs-lookup"><span data-stu-id="ce12f-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

