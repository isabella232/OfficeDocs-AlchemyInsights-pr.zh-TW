---
title: 網域服務的密碼雜湊同步處理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162914"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="42a68-102">網域服務的密碼雜湊同步處理</span><span class="sxs-lookup"><span data-stu-id="42a68-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="42a68-103">**如果您的 Azure AD DS 執行個體提示您啟用密碼雜湊同步處理**</span><span class="sxs-lookup"><span data-stu-id="42a68-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="42a68-104">在內部部署 Azure Active Directory Domain Services (AD DS) 環境同步處理使用者的情況下，您遇到執行混合式環境的情形。</span><span class="sxs-lookup"><span data-stu-id="42a68-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="42a68-105">如果將來自內部部署 AD DS 的密碼雜湊同步處理到 Azure AD 租用戶，就會發生此情況。</span><span class="sxs-lookup"><span data-stu-id="42a68-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="42a68-106">**原因**</span><span class="sxs-lookup"><span data-stu-id="42a68-106">**Cause**</span></span>

<span data-ttu-id="42a68-107">發生這種情況的原因是，Azure AD Connect 預設不會同步處理 Azure AD DS 所需的舊版 New Technology LAN Manager (NTLM) 和 Kerberos 密碼雜湊。</span><span class="sxs-lookup"><span data-stu-id="42a68-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="42a68-108">**因應措施**</span><span class="sxs-lookup"><span data-stu-id="42a68-108">**Workaround**</span></span> 

<span data-ttu-id="42a68-109">您需要設定 Azure AD Connect，以同步處理 NTLM 和 Kerberos 驗證所需的密碼雜湊。</span><span class="sxs-lookup"><span data-stu-id="42a68-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="42a68-110">設定 Azure AD Connect 之後，內部部署帳戶建立或密碼變更事件也會同步處理到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="42a68-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="42a68-111">如需有關此功能的詳細資訊，以及如何在 Azure AD DS 混合式環境中啟用密碼同步處理的指導方針，請參閱[這裡](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)。</span><span class="sxs-lookup"><span data-stu-id="42a68-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>