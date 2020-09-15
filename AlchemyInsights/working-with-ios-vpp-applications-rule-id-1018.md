---
title: 使用 iOS VPP 應用程式規則識別碼1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688937"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="44210-102">使用 iOS VPP 應用程式</span><span class="sxs-lookup"><span data-stu-id="44210-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="44210-103">閱讀 [如何管理透過大量購買程式購買的 iOS 應用程式與 Microsoft intune](https://docs.microsoft.com/intune/vpp-apps-ios) ，以瞭解如何使用 Apple Volume purchase program 的功能、限制和步驟，以及如何在 Microsoft intune 中支援該功能。</span><span class="sxs-lookup"><span data-stu-id="44210-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="44210-104">**常見問題：** 「我將 iOS 的 VPP 應用程式指派給我的使用者，但是安裝失敗。」</span><span class="sxs-lookup"><span data-stu-id="44210-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="44210-105">如果您跨多個行動裝置管理提供者使用單一 VPP 權杖，便會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="44210-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="44210-106">來自 Apple 的 VPP 權杖只會與一個提供者搭配使用。</span><span class="sxs-lookup"><span data-stu-id="44210-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="44210-107">如果您使用的 VPP 權杖與多個提供者，則必須將權杖重新上傳至 Intune。</span><span class="sxs-lookup"><span data-stu-id="44210-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="44210-108">如果安裝總數超過授權數目，也可能會失敗。</span><span class="sxs-lookup"><span data-stu-id="44210-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="44210-109">若要查看授權的流量報告，請移至 [ **Intune 行動應用**程式 \> **應用程式授權** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="44210-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="44210-110">若要瞭解如何回收使用中的授權，請參閱 [本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="44210-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
