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
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>疑難排解 Azure AD 聯結裝置的單一登入

如果您有內部部署 Active Directory (AD) 環境，且想要將您的 AD 網域加入的電腦加入 Azure AD，您可以執行混合式 Azure AD join 以達成此目的。 How [To： Plan the 混合式 Azure Active Directory join 實現](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)提供您在環境中實施混合式 azure AD 聯結的相關步驟。

如需詳細資訊，請參閱 [Configure AZURE AD join 裝置 for 內部部署 Single-Sign on Using Windows Hello 企業版](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)。

**主要更新權杖 (PRT) 問題**

主要重新整理權杖 (PRT) 是 Windows 10、Windows Server 2016 和更新版本、iOS 和 Android 裝置上的 Azure AD 驗證主要專案。 它是一種 JSON Web Token (JWT) 發佈給 Microsoft 第一方權杖代理人，以啟用在這些裝置上所使用之應用程式的單一登入 (SSO) 。 如需如何在 Windows 10 裝置上發行、使用及保護 PRT 的詳細資訊，請參閱 [什麼是主要重新整理權杖？](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)。

**WamDefaultSet： YES 和 AzureADPrt： YES**

這些欄位指出使用者登入裝置時，是否已成功驗證 Azure AD。 如果值是 **NO**，可能是因為：

- 註冊時與裝置相關聯的 TPM 中有壞的儲存金鑰 (請在執行提升) 時檢查 KeySignTest
- 替代登入識別碼
- 找不到 HTTP Proxy

若要使用 dsregcmd 命令來疑難排解裝置，請參閱 [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。
