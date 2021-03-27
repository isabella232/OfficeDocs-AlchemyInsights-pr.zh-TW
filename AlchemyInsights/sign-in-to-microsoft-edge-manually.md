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
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398648"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="0d97c-102">手動登入 Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0d97c-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="0d97c-103">如果使用者在初次執行體驗期間未自動登入，使用者可以透過瀏覽器的設定或 [識別] 浮出控制項手動登入。</span><span class="sxs-lookup"><span data-stu-id="0d97c-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="0d97c-104">若要管理登入，請使用下列原則：</span><span class="sxs-lookup"><span data-stu-id="0d97c-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="0d97c-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) -確保使用者在 Microsoft Edge 中一定會有工作設定檔。</span><span class="sxs-lookup"><span data-stu-id="0d97c-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="0d97c-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -若要限制登入一組信任的帳戶。</span><span class="sxs-lookup"><span data-stu-id="0d97c-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="0d97c-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) -若要停用登入或強制使用者登入。</span><span class="sxs-lookup"><span data-stu-id="0d97c-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

