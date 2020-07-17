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
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931421"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b4769-102">使用 Intune 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="b4769-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b4769-103">使用具有 Intune 的**條件式存取**需要三個步驟：</span><span class="sxs-lookup"><span data-stu-id="b4769-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="b4769-104">建立**符合性原則**（[Android](https://docs.microsoft.com/intune/compliance-policy-create-android)、 [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)、 [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)），以定義在裝置視為相容性之前必須滿足的設定。</span><span class="sxs-lookup"><span data-stu-id="b4769-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b4769-105">例如，裝置的 pin 碼至少必須是6位數，才會被視為相容。</span><span class="sxs-lookup"><span data-stu-id="b4769-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="b4769-106">建立**條件式存取原則**，以定義要保護的資源，以及存取這些資源所需符合的條件。</span><span class="sxs-lookup"><span data-stu-id="b4769-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="b4769-107">[例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)裝置必須先相容才能存取公司的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="b4769-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="b4769-108">確定**相容性原則**和**條件式存取原則**都是以所需的使用者群組為目標。</span><span class="sxs-lookup"><span data-stu-id="b4769-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="b4769-109">這可能需要在 Azure Active Directory 中建立特定的使用者群組。</span><span class="sxs-lookup"><span data-stu-id="b4769-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="b4769-110">**有用的連結：**</span><span class="sxs-lookup"><span data-stu-id="b4769-110">**Helpful links:**</span></span>

[<span data-ttu-id="b4769-111">裝置合規性概述</span><span class="sxs-lookup"><span data-stu-id="b4769-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="b4769-112">疑難排解 CA</span><span class="sxs-lookup"><span data-stu-id="b4769-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="b4769-113">疑難排解原則</span><span class="sxs-lookup"><span data-stu-id="b4769-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="b4769-114">若要保護電子郵件（Exchange online）不受相容裝置存取，必須遵循這兩個檔：</span><span class="sxs-lookup"><span data-stu-id="b4769-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="b4769-115">使用 EAS 保護來自裝置的電子郵件存取</span><span class="sxs-lookup"><span data-stu-id="b4769-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="b4769-116">使用新式驗證用戶端（例如 Outlook）保護從裝置進行的電子郵件存取</span><span class="sxs-lookup"><span data-stu-id="b4769-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)