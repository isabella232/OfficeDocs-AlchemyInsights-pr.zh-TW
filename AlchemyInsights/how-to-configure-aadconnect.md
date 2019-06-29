---
title: 646如何設定 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385321"
---
# <a name="configure-sync-features"></a><span data-ttu-id="27084-102">設定同步處理功能</span><span class="sxs-lookup"><span data-stu-id="27084-102">Configure sync features</span></span>

<span data-ttu-id="27084-103">Azure AD Connect 包含若干預設啟用的功能, 或您可以稍後啟用的功能。</span><span class="sxs-lookup"><span data-stu-id="27084-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="27084-104">某些功能需要在特定環境中進行其他設定。</span><span class="sxs-lookup"><span data-stu-id="27084-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="27084-105">[篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)會限制將物件同步處理至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="27084-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="27084-106">依預設, 會同步處理所有使用者、連絡人、群組及 Windows 10 電腦帳戶。</span><span class="sxs-lookup"><span data-stu-id="27084-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="27084-107">您可以根據網域、Ou 或其他屬性來包含或排除物件。</span><span class="sxs-lookup"><span data-stu-id="27084-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="27084-108">[密碼雜湊同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)處理會將密碼雜湊從內部部署 Active Directory 同步處理至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="27084-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="27084-109">這可讓您在一個位置使用密碼管理, 但在內部部署和雲端環境中使用相同的密碼。</span><span class="sxs-lookup"><span data-stu-id="27084-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="27084-110">因為 Active Directory 是授權來源, 您可以使用自己的密碼原則。</span><span class="sxs-lookup"><span data-stu-id="27084-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="27084-111">[自助密碼重設 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)可讓使用者在自己的內部部署密碼原則中重設自己在雲端中的密碼。</span><span class="sxs-lookup"><span data-stu-id="27084-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="27084-112">[裝置回寫](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)允許 Azure AD 中的註冊裝置被寫回至內部部署 Active Directory, 讓它們可用於條件式存取。</span><span class="sxs-lookup"><span data-stu-id="27084-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="27084-113">[防止意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)預設為啟用, 以協助防止過多的同時刪除物件 (每個同步處理500個以上的物件)。</span><span class="sxs-lookup"><span data-stu-id="27084-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="27084-114">您可以變更此設定, 以符合組織的需求。</span><span class="sxs-lookup"><span data-stu-id="27084-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="27084-115">預設會為快速安裝啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade), 並協助確保您的 Azure AD Connect 版本永遠是最新的。</span><span class="sxs-lookup"><span data-stu-id="27084-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
