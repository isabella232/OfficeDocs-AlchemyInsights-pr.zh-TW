---
title: 使用 iOS VPP 應用程式規則 Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917487"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="4f592-102">使用 iOS VPP 應用程式</span><span class="sxs-lookup"><span data-stu-id="4f592-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="4f592-103">閱讀[如何管理附加元件購買，透過 Microsoft intune 大量購買方案的 iOS 應用程式](https://docs.microsoft.com/intune/vpp-apps-ios)以了解功能、 限制和步驟，請使用 Apple 大量購買方案和其在 Microsoft Intune 的支援。</span><span class="sxs-lookup"><span data-stu-id="4f592-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="4f592-104">**常見問題：**"我指派 iOS VPP 應用程式至我的使用者，但安裝失敗 」。</span><span class="sxs-lookup"><span data-stu-id="4f592-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="4f592-p101">這可以發生如果單一 VPP 權杖跨越多個行動裝置管理提供者。從 Apple VPP 權杖僅搭配一個提供者。如果您是使用 VPP 權杖具有多個提供者，您必須重新上傳至 Intune 的 token。</span><span class="sxs-lookup"><span data-stu-id="4f592-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="4f592-p102">如果安裝總數超過授權數目也會失敗安裝。若要檢視您授權的使用情況報告，請移至**Intune 行動應用程式** \> **應用程式授權**] 頁面。若要了解如何重新取得使用中的授權，請參閱[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="4f592-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

