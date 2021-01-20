---
title: 設定網域服務
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884567"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="003ca-102">無法啟用 AAD-DS 或部署失敗</span><span class="sxs-lookup"><span data-stu-id="003ca-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="003ca-103">若要解決 Azure AD Domain Services (AAD-DS) 未啟用或無法部署的問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="003ca-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="003ca-104">如果您使用的是現有的虛擬網路，請檢查您的 NSG 是否有針對入口網站 https://aka.ms/aadds-networking 中需在 AAD-DS 中同步處理的連接埠封鎖規則。</span><span class="sxs-lookup"><span data-stu-id="003ca-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="003ca-105">請檢查您的錯誤訊息是否在 https://aka.ms/aadds-troubleshoot-enable 中提供的疑難排解指南中得到回覆。</span><span class="sxs-lookup"><span data-stu-id="003ca-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="003ca-106">嘗試在新的虛擬網路中部署 Azure AD Domain Services。</span><span class="sxs-lookup"><span data-stu-id="003ca-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="003ca-107">根據快速入門手冊以了解如何部署 AAD-DS：[建立及設定 AAD 網域服務](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)。</span><span class="sxs-lookup"><span data-stu-id="003ca-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="003ca-108">如果您在部署 Azure AD Domain Services 時發生問題，請參閱 [疑難排解 Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) 以解決常見錯誤即協助您再次進行工作。</span><span class="sxs-lookup"><span data-stu-id="003ca-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="003ca-109">**無法停用 AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="003ca-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="003ca-110">無法暫停 AAD-DS。</span><span class="sxs-lookup"><span data-stu-id="003ca-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="003ca-111">如果您想要停止使用受管理的網域，必須先將它刪除。</span><span class="sxs-lookup"><span data-stu-id="003ca-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="003ca-112">若要刪除受管理的網域，請參閱 [刪除 AAD 網域服務](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)。</span><span class="sxs-lookup"><span data-stu-id="003ca-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



