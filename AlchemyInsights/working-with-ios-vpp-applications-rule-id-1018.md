---
title: 使用 iOS VPP 應用程式規則識別碼1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364835"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="d27a8-102">使用 iOS VPP 應用程式</span><span class="sxs-lookup"><span data-stu-id="d27a8-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="d27a8-103">請參閱[如何使用 Microsoft intune 的大量購買程式來管理已購買的 iOS 應用程式](https://docs.microsoft.com/intune/vpp-apps-ios), 以瞭解功能、限制, 以及如何使用 Apple 大量購買程式, 以及如何在 Microsoft Intune 中支援。</span><span class="sxs-lookup"><span data-stu-id="d27a8-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="d27a8-104">**常見問題:**「我將 iOS VPP 應用程式指派給我的使用者, 但安裝失敗。」</span><span class="sxs-lookup"><span data-stu-id="d27a8-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="d27a8-105">如果在多個行動裝置管理提供者上使用單一 VPP 權杖, 就會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="d27a8-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="d27a8-106">來自 Apple 的 VPP 權杖只能與一個提供者搭配使用。</span><span class="sxs-lookup"><span data-stu-id="d27a8-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="d27a8-107">如果您將 VPP 權杖與多個提供者搭配使用, 則必須將 token 重新上傳至 Intune。</span><span class="sxs-lookup"><span data-stu-id="d27a8-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="d27a8-108">如果安裝總數超過授權數目, 安裝也會失敗。</span><span class="sxs-lookup"><span data-stu-id="d27a8-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="d27a8-109">若要查看您的授權使用方式報告, 請移至 [ **Intune 行動應用** \> **程式應用程式授權**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="d27a8-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="d27a8-110">若要瞭解如何收回使用中的授權, 請參閱[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="d27a8-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
