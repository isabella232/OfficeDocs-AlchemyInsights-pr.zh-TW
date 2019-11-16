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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/15/2019
ms.locfileid: "36504985"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e506b-102">使用 Intune 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="e506b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e506b-103">使用 Intune 使用**條件式存取**需要 3 個步驟：</span><span class="sxs-lookup"><span data-stu-id="e506b-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e506b-104">建立一個**條件式存取原則**來定義哪些資源會受到保護，以及條件必須符合要存取這些資源。</span><span class="sxs-lookup"><span data-stu-id="e506b-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="e506b-105">例如，裝置必須符合之前存取公司電子郵件。</span><span class="sxs-lookup"><span data-stu-id="e506b-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e506b-106">建立**符合性原則**來定義必須先符合裝置會被視為相容的設定。</span><span class="sxs-lookup"><span data-stu-id="e506b-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e506b-107">例如，裝置必須至少 6 位數字的 pin 碼之前會被視為相容。</span><span class="sxs-lookup"><span data-stu-id="e506b-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e506b-108">確保**符合性原則**和**條件式存取原則**的目標的使用者所需的群組。</span><span class="sxs-lookup"><span data-stu-id="e506b-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="e506b-109">這可能需要在 Azure Active Directory 中建立特定使用者群組。</span><span class="sxs-lookup"><span data-stu-id="e506b-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e506b-110">深入了解：</span><span class="sxs-lookup"><span data-stu-id="e506b-110">Read more:</span></span>
  
- [<span data-ttu-id="e506b-111">條件式存取的最佳作法</span><span class="sxs-lookup"><span data-stu-id="e506b-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e506b-112">開始使用條件式存取</span><span class="sxs-lookup"><span data-stu-id="e506b-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

