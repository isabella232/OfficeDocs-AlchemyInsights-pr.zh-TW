---
title: 設定格式化的條件 intune 的存取
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278326"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="446dc-102">設定格式化的條件 intune 的存取</span><span class="sxs-lookup"><span data-stu-id="446dc-102">Conditional Access with Intune</span></span>

<span data-ttu-id="446dc-103">使用**設定格式化的條件存取**intune 需要 3 個步驟：</span><span class="sxs-lookup"><span data-stu-id="446dc-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="446dc-p101">建立定義哪些資源所要受到保護，而需要存取這些資源符合的條件的**設定格式化的條件存取原則**。例如，裝置必須符合才存取公司的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="446dc-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="446dc-p102">建立**規範原則**定義裝置會被視為相容前必須符合的設定。例如，裝置必須至少 6 位數的 pin 才會視為相容。</span><span class="sxs-lookup"><span data-stu-id="446dc-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="446dc-p103">確保**規範遵守原則**和**設定格式化的條件存取原則**會針對所需的使用者群組。這可能需要在 Azure Active Directory 中建立特定使用者群組。</span><span class="sxs-lookup"><span data-stu-id="446dc-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="446dc-110">閱讀更多：</span><span class="sxs-lookup"><span data-stu-id="446dc-110">Read more:</span></span>
  
- [<span data-ttu-id="446dc-111">條件式存取的最佳作法</span><span class="sxs-lookup"><span data-stu-id="446dc-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="446dc-112">條件式存取的快速入門</span><span class="sxs-lookup"><span data-stu-id="446dc-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

