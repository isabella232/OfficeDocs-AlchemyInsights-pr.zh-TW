---
title: 對來賓使用者問題進行疑難排解
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939370"
---
# <a name="troubleshoot-guest-user-issues"></a>對來賓使用者問題進行疑難排解

1. 如需管理對應用程式之來賓存取的指導方針，請參閱 [Manage guest access With AZURE AD access 評論](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)。
1. 在[azure 入口網站中將來賓使用者新增至您的目錄](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)：在此快速入門中，您將透過 azure 入口網站將新的來賓使用者新增至 azure AD 目錄、傳送邀請，以及查看來賓使用者的邀請兌換處理常式的外觀。
1. [Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)：在此快速入門中，您將使用 New-AzureADMSInvitation 命令，將一個來賓使用者新增至您的 Azure 租使用者。
1. 若要瞭解如何將使用者和群組指派給 Azure Active Directory (azure AD) 中的企業應用程式，請從 azure 入口網站或使用 PowerShell，參閱在[Azure Active Directory 中管理應用程式的使用者指派](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)。 
1. Azure Active Directory (azure ad) B2B 共同作業可搭配大多數與 Azure AD 整合的應用程式使用。 在 [本文](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)中，我們將逐步逐步說明如何設定一些流行的 SaaS 應用程式，以搭配 Azure AD B2B 使用。
1. 作為使用 Azure Active Directory (azure ad) B2B 共同作業功能的組織，將來賓使用者從夥伴組織邀請至您的 Azure ad，您現在可以提供這些 B2B 使用者存取內部部署應用程式。 這些內部部署應用程式可使用 SAML-based 驗證或整合式 Windows 驗證 (IWA) 與 Kerberos 限制委派 (KCD) 。 如需詳細資訊，請參閱在 [AZURE AD 中授與 B2B 使用者內部部署應用程式的存取權](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)。
1. 瞭解如何 [使用 AZURE AD B2B 共同作業，授與受管理的本機夥伴帳戶對雲端資源的存取權](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)。