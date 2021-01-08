---
title: 資訊安全中心的找不到訂閱訊息
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768419"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="ea28e-102">資訊安全中心的找不到訂閱訊息</span><span class="sxs-lookup"><span data-stu-id="ea28e-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="ea28e-103">如果在存取 Microsoft Defender 資訊安全中心時收到「找不到訂閱」訊息，表示用來將該使用者登入入口網站的 Azure Active Directory (AAD) 沒有 Microsoft Defender ATP 授權。</span><span class="sxs-lookup"><span data-stu-id="ea28e-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="ea28e-104">Windows E5 和 Office E5 授權是不同的授權。</span><span class="sxs-lookup"><span data-stu-id="ea28e-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="ea28e-105">如果已購買授權，但該授權未佈建給此 AAD 執行個體，請開啟支援案例。</span><span class="sxs-lookup"><span data-stu-id="ea28e-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="ea28e-106">您可能發生以下兩個情況之一：</span><span class="sxs-lookup"><span data-stu-id="ea28e-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="ea28e-107">可能發生授權佈建問題。</span><span class="sxs-lookup"><span data-stu-id="ea28e-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="ea28e-108">您不慎將授權佈建給與用來向服務進行驗證的 Microsoft AAD 不同的 Microsoft AAD。</span><span class="sxs-lookup"><span data-stu-id="ea28e-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>