---
title: 網域控制站
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886800"
---
# <a name="domain-controller"></a><span data-ttu-id="c2638-102">網域控制站</span><span class="sxs-lookup"><span data-stu-id="c2638-102">Domain controller</span></span>

<span data-ttu-id="c2638-103">**無法啟用 AAD-DS 或部署失敗**</span><span class="sxs-lookup"><span data-stu-id="c2638-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="c2638-104">若要解決未啟用或無法部署 Azure AD domain service (AAD-DS) 的問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="c2638-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="c2638-105">如果您正在使用現有的虛擬網路，請檢查您的 NSG 是否有針對入口網站 https://aka.ms/aadds-networking 中需在 AAD-DS 中同步處理的連接埠封鎖規則。</span><span class="sxs-lookup"><span data-stu-id="c2638-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="c2638-106">請檢查您的錯誤訊息是否在 https://aka.ms/aadds-troubleshoot-enable 中提供的疑難排解指南中得到回覆。</span><span class="sxs-lookup"><span data-stu-id="c2638-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="c2638-107">嘗試在新的虛擬網路中部署 Azure AD Domain Services。</span><span class="sxs-lookup"><span data-stu-id="c2638-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="c2638-108">根據快速入門手冊以了解如何部署 AAD-DS，可在 [建立 Azure AD Domain Services 教學課程](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance) 取得。</span><span class="sxs-lookup"><span data-stu-id="c2638-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="c2638-109">如果您在部署 Azure AD Domain Services 時發生問題，請參閱 [疑難排解 Azure AD Domain Services ](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) 解決常見錯誤，以協助您再次進行工作。</span><span class="sxs-lookup"><span data-stu-id="c2638-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="c2638-110">**無法停用 AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="c2638-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="c2638-111">無法暫停 AAD-DS。</span><span class="sxs-lookup"><span data-stu-id="c2638-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="c2638-112">如果您想要停止使用受管理的網域，必須先將它刪除。</span><span class="sxs-lookup"><span data-stu-id="c2638-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="c2638-113">如果您遇到問題，若要解決常見的錯誤訊息，以及相關的疑難排解步驟，以協助您再次執行工作，請參閱 [疑難排解 Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)。</span><span class="sxs-lookup"><span data-stu-id="c2638-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
