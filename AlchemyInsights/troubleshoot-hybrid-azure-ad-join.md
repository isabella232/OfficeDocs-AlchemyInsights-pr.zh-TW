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
# <a name="troubleshoot-hybrid-azure-ad-join"></a>疑難排解混合式 Azure AD Join

強烈建議確保裝置可以使用 [Device Registration Connectivity 指令碼](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)存取系統帳戶下的裝置註冊端點。

1. 如果您是第一次設定裝置註冊，請務必查看[Azure Active Directory 中的裝置管理簡介](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)，以了解如何取得受 Azure AD 控制的裝置。
1. 如果您直接將裝置註冊到 Azure AD，並註冊到 Intune，請確定您 [已設定 Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ，並先將 [授權](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 就位。
1. 請確保您獲得授權，可以在 Azure AD 和內部部署 AD 中執行作業。 只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。 此外，如果您要在 Windows Server Active Directory 中設定自動註冊，您必須是 Active Directory 和 AD FS 的系統管理員 (如果適用)。

有關解決混合式加入的潛在問題的詳細資訊，請參閱 [疑難排解混合式加入](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) 以設定已加入混合式 Azure AD，而使用 Azure Ad 入口網站管理裝置，則參閱 [設定已加入混合式 Azure AD (已加入內部部署網域) 裝置](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) 和 [使用 Azure 入口網站管理裝置](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。

若要解決混合式 Azure Active Directory (AD) Join 常見問題，請參閱[混合式 Azure AD Join 常見問題](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)。
