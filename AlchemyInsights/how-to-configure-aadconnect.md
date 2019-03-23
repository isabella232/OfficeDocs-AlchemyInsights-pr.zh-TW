---
title: 646 如何設定 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779503"
---
# <a name="configure-sync-features"></a><span data-ttu-id="c9642-102">設定同步處理功能</span><span class="sxs-lookup"><span data-stu-id="c9642-102">Configure sync features</span></span>

<span data-ttu-id="c9642-103">Azure AD Connect 包含數個功能，已啟用根據預設，或更新版本，您可以啟用。</span><span class="sxs-lookup"><span data-stu-id="c9642-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="c9642-104">有些功能需要在特定環境的其他設定。</span><span class="sxs-lookup"><span data-stu-id="c9642-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="c9642-105">[篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制物件同步處理到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="c9642-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="c9642-106">依預設，所有使用者、 連絡人、 群組及 Windows 10 電腦帳戶已同步處理。</span><span class="sxs-lookup"><span data-stu-id="c9642-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="c9642-107">您可以包含或排除依據網域、 Ou、 或其他屬性的物件。</span><span class="sxs-lookup"><span data-stu-id="c9642-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="c9642-108">[密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)會同步處理到 Azure AD 從內部部署 Active Directory 密碼雜湊。</span><span class="sxs-lookup"><span data-stu-id="c9642-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="c9642-109">這可讓密碼管理在一個位置，但使用相同的密碼，在這兩個內部部署和雲端環境。</span><span class="sxs-lookup"><span data-stu-id="c9642-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="c9642-110">因為 Active Directory 的授權來源，您可以使用您自己的密碼原則。</span><span class="sxs-lookup"><span data-stu-id="c9642-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="c9642-111">[自助式密碼重設 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)允許使用者自行重設密碼定域機組中的時，仍然套用您內部部署的密碼原則。</span><span class="sxs-lookup"><span data-stu-id="c9642-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="c9642-112">[裝置寫回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)寫回至內部部署 Active Directory 讓他們可以使用條件式存取的 Azure AD 中允許已註冊的裝置。</span><span class="sxs-lookup"><span data-stu-id="c9642-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="c9642-113">[防止意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)預設會啟用，協助防範太多同時刪除的物件 （同步處理每個超過 500 個物件）。</span><span class="sxs-lookup"><span data-stu-id="c9642-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="c9642-114">您可以變更此設定以符合組織的需求。</span><span class="sxs-lookup"><span data-stu-id="c9642-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="c9642-115">快速安裝預設會啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)，以協助確保您的 Azure AD Connect 版本永遠是最新。</span><span class="sxs-lookup"><span data-stu-id="c9642-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

