---
title: 網域服務同步處理
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876514"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="1dd4e-102">網域服務同步處理</span><span class="sxs-lookup"><span data-stu-id="1dd4e-102">Domain service synchronization</span></span>

<span data-ttu-id="1dd4e-103">在 Azure Active Directory 網域服務中 (Azure AD DS) 受管理網域中的物件和認證，可在網域內的本機建立，或從 Azure Active (Directory) 租使用者同步處理。</span><span class="sxs-lookup"><span data-stu-id="1dd4e-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="1dd4e-104">當您第一次部署 Azure AD DS 時，會設定並啟動自動單向同步處理，以從 Azure AD 複製物件。</span><span class="sxs-lookup"><span data-stu-id="1dd4e-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="1dd4e-105">這種單向同步處理會繼續在後臺執行，使 Azure AD DS 管理網域與 Azure AD 中的任何變更保持最新狀態。</span><span class="sxs-lookup"><span data-stu-id="1dd4e-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="1dd4e-106">Azure AD DS 之間不會進行同步處理傳回 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="1dd4e-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="1dd4e-107">如需 Azure Active Directory 網域服務同步處理的詳細資訊，請參閱 [網域服務同步](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)處理。</span><span class="sxs-lookup"><span data-stu-id="1dd4e-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
