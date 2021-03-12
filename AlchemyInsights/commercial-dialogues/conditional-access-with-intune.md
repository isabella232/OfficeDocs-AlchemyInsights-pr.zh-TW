---
title: 使用 Intune 的條件式存取
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735996"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="21fd4-102">使用 Intune 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="21fd4-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="21fd4-103">使用具有 Intune 的條件式存取需要三個步驟：</span><span class="sxs-lookup"><span data-stu-id="21fd4-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="21fd4-104">建立相容性原則，以定義在將裝置視為合規性之前必須滿足的設定。例如，裝置的 pin 碼至少必須是6位數，才會被視為相容。</span><span class="sxs-lookup"><span data-stu-id="21fd4-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="21fd4-105">建立條件式存取原則，以定義要保護的資源，以及存取這些資源所需符合的條件。例如，裝置必須先相容才能存取公司的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="21fd4-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="21fd4-106">確定相容性原則和條件式存取原則都是以所需的使用者群組為目標。這可能需要在 Azure Active Directory 中建立特定的使用者群組。</span><span class="sxs-lookup"><span data-stu-id="21fd4-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="21fd4-107">閱讀其他資訊...</span><span class="sxs-lookup"><span data-stu-id="21fd4-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
