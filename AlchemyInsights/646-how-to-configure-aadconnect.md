---
title: 646 如何設定 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499661"
---
# <a name="configure-sync-features"></a><span data-ttu-id="c9a4a-102">設定同步處理功能</span><span class="sxs-lookup"><span data-stu-id="c9a4a-102">Configure sync features</span></span>

<span data-ttu-id="c9a4a-p101">Azure AD 連接包含數項功能的啟用根據預設，或您可以稍後啟用。有些功能需要特定的環境中的其他設定。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="c9a4a-p102">[篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制物件已同步處理至 Azure AD。依預設，所有使用者、 連絡人、 群組及 Windows 10 進行同步處理電腦帳戶。您可以包含或排除物件根據網域、 Ou、 或其他屬性。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="c9a4a-p103">[密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)會從內部部署 Active Directory 至 Azure AD 的密碼雜湊同步處理。這可讓密碼管理的單一位置，但是相同的密碼中同時使用內部部署和雲端環境。因為 Active Directory 的授權來源，您可以使用自己的密碼原則。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="c9a4a-111">[自助式密碼重設 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)可讓使用者在雲端自己密碼重設時仍套用您內部部署的密碼原則。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="c9a4a-112">[裝置回寫](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)可寫入回內部部署 Active Directory 讓他們可以用於設定格式化的條件存取 Azure AD 中的已登錄的裝置。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="c9a4a-p104">[避免意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)預設會啟用以協助防止太多同時物件刪除 （同步處理個別超過 500 個物件）。您可以變更此設定可符合組織的需求。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="c9a4a-115">Express 安裝預設會啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)並有助於確保您的 Azure AD 連接版本永遠是最新。</span><span class="sxs-lookup"><span data-stu-id="c9a4a-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

