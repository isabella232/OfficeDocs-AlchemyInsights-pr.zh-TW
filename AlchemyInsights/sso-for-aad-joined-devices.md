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
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>已加入 Azure Active Directory 裝置的單一登入

如果您有內部部署 Active Directory (AD) 環境，且想要將您的 AD 網域加入的電腦加入 Azure AD，您可以執行混合式 Azure AD join 以達成此目的。 How [To： Plan the 混合式 Azure Active Directory join 實現](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)提供您在環境中實施混合式 azure AD 聯結的相關步驟。

[使用 Windows Hello 企業版為內部部署 Single-Sign 設定 Azure AD 加入的裝置](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**主要更新權杖 (PRT) 問題** 主要重新整理權杖 (PRT) 是 Windows 10、Windows Server 2016 和更新版本、iOS 和 Android 裝置上的 Azure AD 驗證主要專案。 它是一種 JSON Web Token (JWT) 發佈給 Microsoft 第一方權杖代理人，以啟用在這些裝置上所使用之應用程式的單一登入 (SSO) 。 [在什麼是主要重新整理權杖？](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)中，我們將提供有關如何在 Windows 10 裝置上發行、使用及保護 PRT 的詳細資訊。

**WamDefaultSet： yes 和 AzureADPrt： yes** 這些欄位指出使用者登入裝置時，是否已成功驗證 Azure AD。 如果值為 [ **否**]，則可能是由於下列原因：

- 註冊時與裝置相關聯的 TPM 中有壞的儲存金鑰 (請在執行提升的) 時，檢查 KeySignTest。
- 替代登入識別碼
- 找不到 HTTP Proxy

使用 dsregcmd 命令- [SSO 狀態](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)進行裝置疑難排解
