---
title: 啟用裝置
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
- "8278"
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003465"
---
# <a name="enable-device"></a>啟用裝置

**啟用裝置使用 Powershell 命令**

執行下列命令：

- 若要取得 device 物件： `Get-MsolDevice -Name <Name>`
- 若要啟用裝置： `Enable-MsolDevice -DeviceId <DeviceId>`

如需在受管理的網域上設定混合式加入的詳細資訊，請參閱 [設定混合式加入](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)。
