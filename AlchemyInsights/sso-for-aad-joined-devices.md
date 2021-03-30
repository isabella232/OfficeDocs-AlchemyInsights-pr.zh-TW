---
title: 適用于 Azure Active Directory 已加入裝置的 Single-Sign
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403781"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="a025e-102">已加入 Azure Active Directory 裝置的單一登入</span><span class="sxs-lookup"><span data-stu-id="a025e-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="a025e-103">如果您有內部部署 Active Directory (AD) 環境，且想要將您的 AD 網域加入的電腦加入 Azure AD，您可以執行混合式 Azure AD join 以達成此目的。</span><span class="sxs-lookup"><span data-stu-id="a025e-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="a025e-104">How [To： Plan the 混合式 Azure Active Directory join 實現](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)提供您在環境中實施混合式 azure AD 聯結的相關步驟。</span><span class="sxs-lookup"><span data-stu-id="a025e-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="a025e-105">使用 Windows Hello 企業版為內部部署 Single-Sign 設定 Azure AD 加入的裝置</span><span class="sxs-lookup"><span data-stu-id="a025e-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="a025e-106">**主要更新權杖 (PRT) 問題** 主要重新整理權杖 (PRT) 是 Windows 10、Windows Server 2016 和更新版本、iOS 和 Android 裝置上的 Azure AD 驗證主要專案。</span><span class="sxs-lookup"><span data-stu-id="a025e-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="a025e-107">它是一種 JSON Web Token (JWT) 發佈給 Microsoft 第一方權杖代理人，以啟用在這些裝置上所使用之應用程式的單一登入 (SSO) 。</span><span class="sxs-lookup"><span data-stu-id="a025e-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="a025e-108">[在什麼是主要重新整理權杖？](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)中，我們將提供有關如何在 Windows 10 裝置上發行、使用及保護 PRT 的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="a025e-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="a025e-109">**WamDefaultSet： yes 和 AzureADPrt： yes** 這些欄位指出使用者登入裝置時，是否已成功驗證 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="a025e-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="a025e-110">如果值為 [ **否**]，則可能是由於下列原因：</span><span class="sxs-lookup"><span data-stu-id="a025e-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="a025e-111">註冊時與裝置相關聯的 TPM 中有壞的儲存金鑰 (請在執行提升的) 時，檢查 KeySignTest。</span><span class="sxs-lookup"><span data-stu-id="a025e-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="a025e-112">替代登入識別碼</span><span class="sxs-lookup"><span data-stu-id="a025e-112">Alternate Login ID</span></span>
- <span data-ttu-id="a025e-113">找不到 HTTP Proxy</span><span class="sxs-lookup"><span data-stu-id="a025e-113">HTTP Proxy not found</span></span>

<span data-ttu-id="a025e-114">使用 dsregcmd 命令- [SSO 狀態](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)進行裝置疑難排解</span><span class="sxs-lookup"><span data-stu-id="a025e-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
