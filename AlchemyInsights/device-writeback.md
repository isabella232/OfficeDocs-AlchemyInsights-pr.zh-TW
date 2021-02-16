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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255148"
---
# <a name="device-writeback"></a>裝置回寫

在下列情況下，會使用裝置回寫：

- [使用混合式憑證信任部署來啟用 Windows Hello 企業版](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- 根據裝置到 ADFS (2012 R2 或更高) 受保護的應用程式 (信賴憑證者信任，啟用條件式存取) 

    > [!NOTE]
    > 裝置回寫需要使用 Azure AD Premium 訂閱。

這提供額外的安全性並保證僅將應用程式的存取權授與信任的裝置。 如需條件式存取的詳細資訊，請參閱[使用 Azure Active Directory 裝置註冊](https://docs.microsoft.com/azure/active-directory/devices/overview)[管理具有條件存取的風險](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)及設定內部部署條件式存取。

如需啟用裝置的裝置回寫功能的詳細資訊，請參閱 [Enable Device 回寫](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)。
