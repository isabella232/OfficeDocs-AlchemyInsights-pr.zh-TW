---
title: 疑難排解混合式 Azure AD Join
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401898"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="a4aa5-102">疑難排解混合式 Azure AD Join</span><span class="sxs-lookup"><span data-stu-id="a4aa5-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="a4aa5-103">強烈建議確保裝置可以使用 [Device Registration Connectivity 指令碼](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)存取系統帳戶下的裝置註冊端點。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="a4aa5-104">如果您是第一次設定裝置註冊，請務必查看[Azure Active Directory 中的裝置管理簡介](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)，以了解如何取得受 Azure AD 控制的裝置。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="a4aa5-105">如果您直接將裝置註冊到 Azure AD，並註冊到 Intune，請確定您 [已設定 Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ，並先將 [授權](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 就位。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="a4aa5-106">請確保您獲得授權，可以在 Azure AD 和內部部署 AD 中執行作業。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="a4aa5-107">只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="a4aa5-108">此外，如果您要在 Windows Server Active Directory 中設定自動註冊，您必須是 Active Directory 和 AD FS 的系統管理員 (如果適用)。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="a4aa5-109">有關解決混合式加入的潛在問題的詳細資訊，請參閱 [疑難排解混合式加入](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) 以設定已加入混合式 Azure AD，而使用 Azure Ad 入口網站管理裝置，則參閱 [設定已加入混合式 Azure AD (已加入內部部署網域) 裝置](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) 和 [使用 Azure 入口網站管理裝置](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a4aa5-110">若要解決混合式 Azure Active Directory (AD) Join 常見問題，請參閱[混合式 Azure AD Join 常見問題](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)。</span><span class="sxs-lookup"><span data-stu-id="a4aa5-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
