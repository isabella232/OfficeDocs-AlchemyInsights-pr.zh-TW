---
title: 疑難排解 Azure AD 聯結裝置的單一登入
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897742"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="1734c-102">疑難排解 Azure AD 聯結裝置的單一登入</span><span class="sxs-lookup"><span data-stu-id="1734c-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="1734c-103">如果您有內部部署 Active Directory (AD) 環境，且想要將您的 AD 網域加入的電腦加入 Azure AD，您可以執行混合式 Azure AD join 以達成此目的。</span><span class="sxs-lookup"><span data-stu-id="1734c-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="1734c-104">How [To： Plan the 混合式 Azure Active Directory join 實現](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)提供您在環境中實施混合式 azure AD 聯結的相關步驟。</span><span class="sxs-lookup"><span data-stu-id="1734c-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="1734c-105">如需詳細資訊，請參閱 [Configure AZURE AD join 裝置 for 內部部署 Single-Sign on Using Windows Hello 企業版](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)。</span><span class="sxs-lookup"><span data-stu-id="1734c-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="1734c-106">**主要更新權杖 (PRT) 問題**</span><span class="sxs-lookup"><span data-stu-id="1734c-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="1734c-107">主要重新整理權杖 (PRT) 是 Windows 10、Windows Server 2016 和更新版本、iOS 和 Android 裝置上的 Azure AD 驗證主要專案。</span><span class="sxs-lookup"><span data-stu-id="1734c-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="1734c-108">它是一種 JSON Web Token (JWT) 發佈給 Microsoft 第一方權杖代理人，以啟用在這些裝置上所使用之應用程式的單一登入 (SSO) 。</span><span class="sxs-lookup"><span data-stu-id="1734c-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="1734c-109">如需如何在 Windows 10 裝置上發行、使用及保護 PRT 的詳細資訊，請參閱 [什麼是主要重新整理權杖？](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)。</span><span class="sxs-lookup"><span data-stu-id="1734c-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="1734c-110">**WamDefaultSet： YES 和 AzureADPrt： YES**</span><span class="sxs-lookup"><span data-stu-id="1734c-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="1734c-111">這些欄位指出使用者登入裝置時，是否已成功驗證 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="1734c-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="1734c-112">如果值是 **NO**，可能是因為：</span><span class="sxs-lookup"><span data-stu-id="1734c-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="1734c-113">註冊時與裝置相關聯的 TPM 中有壞的儲存金鑰 (請在執行提升) 時檢查 KeySignTest</span><span class="sxs-lookup"><span data-stu-id="1734c-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="1734c-114">替代登入識別碼</span><span class="sxs-lookup"><span data-stu-id="1734c-114">Alternate Login ID</span></span>
- <span data-ttu-id="1734c-115">找不到 HTTP Proxy</span><span class="sxs-lookup"><span data-stu-id="1734c-115">HTTP Proxy not found</span></span>

<span data-ttu-id="1734c-116">若要使用 dsregcmd 命令來疑難排解裝置，請參閱 [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。</span><span class="sxs-lookup"><span data-stu-id="1734c-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
