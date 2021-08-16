---
title: 裝置回寫
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101941"
---
# <a name="device-writeback"></a>裝置回寫

在下列情況下，會使用裝置回寫：

- [使用混合式憑證信任部署來啟用商務 Windows Hello](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- 根據裝置到 ADFS (2012 R2 或更高) 受保護的應用程式 (信賴憑證者信任，啟用條件式存取) 

    > [!NOTE]
    > 裝置回寫需要 Azure AD Premium 訂閱。

這提供額外的安全性並保證僅將應用程式的存取權授與信任的裝置。 如需條件式存取的詳細資訊，請參閱使用[條件式存取管理風險](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)及[設定內部部署條件式存取使用 Azure Active Directory 裝置註冊](https://docs.microsoft.com/azure/active-directory/devices/overview)。

如需啟用裝置的裝置回寫功能的詳細資訊，請參閱 [Enable Device 回寫](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)。
