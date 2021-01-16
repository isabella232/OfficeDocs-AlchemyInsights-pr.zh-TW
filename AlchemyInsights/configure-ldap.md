---
title: 設定 LDAP
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
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876549"
---
# <a name="configure-ldap"></a><span data-ttu-id="78827-102">設定 LDAP</span><span class="sxs-lookup"><span data-stu-id="78827-102">Configure LDAP</span></span>

<span data-ttu-id="78827-103">若要設定 LDAP，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="78827-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="78827-104">檢查 [Azure 入口網站](https://aka.ms/aadds-health)上網域的健康情況。</span><span class="sxs-lookup"><span data-stu-id="78827-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="78827-105">請確定有效的 Azure AD 訂閱可供使用，且已啟用 Azure AD 網域服務。</span><span class="sxs-lookup"><span data-stu-id="78827-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="78827-106">啟用安全 LDAP 所需的憑證必須從信任的公用憑證授權單位單位取得，或是由自我簽署的憑證取得。</span><span class="sxs-lookup"><span data-stu-id="78827-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="78827-107">確定憑證遵循必要的 [指導方針](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)。</span><span class="sxs-lookup"><span data-stu-id="78827-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="78827-108">**不正確憑證**</span><span class="sxs-lookup"><span data-stu-id="78827-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="78827-109">若要更新憑證，請依照下列步驟建立新的憑證和 reupload： [CONFIGURE LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="78827-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="78827-110">若要在 Azure Active directory 網域服務中解決安全 LDAP 警示的已知問題，請參閱 [解決 LDAP 警示](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="78827-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
