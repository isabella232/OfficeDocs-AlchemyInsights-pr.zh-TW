---
title: 手動登入 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f9aa27a585d805360e1fadecfd0db3b11d15a3594ed5bd5dc6c68cec37a4d6a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050757"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>手動登入 Microsoft Edge

如果使用者在初次執行體驗期間未自動登入，使用者可以透過瀏覽器的設定或 [識別] 浮出控制項手動登入。 若要管理登入，請使用下列原則：

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -確保使用者在 Microsoft Edge 中一定會有工作設定檔。
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -若要限制登入一組信任的帳戶。
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -若要停用登入或強制使用者登入。

