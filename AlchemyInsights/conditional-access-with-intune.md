---
title: 使用 Intune 的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706012"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="962fb-102">使用 Intune 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="962fb-102">Conditional Access with Intune</span></span>

<span data-ttu-id="962fb-103">使用具有 Intune 的**條件式存取**需要三個步驟：</span><span class="sxs-lookup"><span data-stu-id="962fb-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="962fb-104">建立**條件式存取原則**，以定義要保護的資源，以及存取這些資源所需符合的條件。</span><span class="sxs-lookup"><span data-stu-id="962fb-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="962fb-105">例如，裝置必須先相容才能存取公司的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="962fb-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="962fb-106">建立**相容性原則**，以定義在將裝置視為合規性之前必須滿足的設定。</span><span class="sxs-lookup"><span data-stu-id="962fb-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="962fb-107">例如，裝置的 pin 碼至少必須是6位數，才會被視為相容。</span><span class="sxs-lookup"><span data-stu-id="962fb-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="962fb-108">確保**相容性原則**和**條件式存取原則**都是以所需的使用者群組為目標。</span><span class="sxs-lookup"><span data-stu-id="962fb-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="962fb-109">這可能需要在 Azure Active Directory 中建立特定的使用者群組。</span><span class="sxs-lookup"><span data-stu-id="962fb-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="962fb-110">閱讀其他資訊：</span><span class="sxs-lookup"><span data-stu-id="962fb-110">Read more:</span></span>
  
- [<span data-ttu-id="962fb-111">條件式存取的最佳作法</span><span class="sxs-lookup"><span data-stu-id="962fb-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="962fb-112">條件式存取快速入門</span><span class="sxs-lookup"><span data-stu-id="962fb-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

