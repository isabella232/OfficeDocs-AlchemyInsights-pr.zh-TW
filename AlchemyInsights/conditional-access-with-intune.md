---
title: 使用 Intune 的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393532"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="1f53a-102">使用 Intune 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="1f53a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="1f53a-103">使用 Intune 使用**條件式存取**需要 3 個步驟：</span><span class="sxs-lookup"><span data-stu-id="1f53a-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="1f53a-104">建立一個**條件式存取原則**來定義哪些資源會受到保護，以及條件必須符合要存取這些資源。</span><span class="sxs-lookup"><span data-stu-id="1f53a-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="1f53a-105">例如，裝置必須符合之前存取公司電子郵件。</span><span class="sxs-lookup"><span data-stu-id="1f53a-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="1f53a-106">建立**符合性原則**來定義必須先符合裝置會被視為相容的設定。</span><span class="sxs-lookup"><span data-stu-id="1f53a-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="1f53a-107">例如，裝置必須至少 6 位數字的 pin 碼之前會被視為相容。</span><span class="sxs-lookup"><span data-stu-id="1f53a-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="1f53a-108">確保**符合性原則**和**條件式存取原則**的目標的使用者所需的群組。</span><span class="sxs-lookup"><span data-stu-id="1f53a-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="1f53a-109">這可能需要在 Azure Active Directory 中建立特定使用者群組。</span><span class="sxs-lookup"><span data-stu-id="1f53a-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="1f53a-110">深入了解：</span><span class="sxs-lookup"><span data-stu-id="1f53a-110">Read more:</span></span>
  
- [<span data-ttu-id="1f53a-111">條件式存取的最佳作法</span><span class="sxs-lookup"><span data-stu-id="1f53a-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="1f53a-112">開始使用條件式存取</span><span class="sxs-lookup"><span data-stu-id="1f53a-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

