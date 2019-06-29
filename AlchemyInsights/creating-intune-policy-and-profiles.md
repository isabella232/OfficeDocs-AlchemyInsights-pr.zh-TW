---
title: 建立 Intune 原則和設定檔
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 580903fd89dca8a2ecbf635fa2157f31c93b85f4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363752"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="5eca9-102">建立 Intune 原則和設定檔</span><span class="sxs-lookup"><span data-stu-id="5eca9-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="5eca9-103">在 Intune 中, 您可以建立執行不同事項的原則和設定檔。</span><span class="sxs-lookup"><span data-stu-id="5eca9-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="5eca9-104">**註冊設定檔**: 依平臺預先配置裝置、啟用使用者相關性、使用多重要素驗證等等。</span><span class="sxs-lookup"><span data-stu-id="5eca9-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="5eca9-105">[何謂裝置註冊](https://docs.microsoft.com/intune/device-enrollment), 以及建立[Android](https://docs.microsoft.com/intune/android-enroll)、 [iOS](https://docs.microsoft.com/intune/ios-enroll)、 [macOS](https://docs.microsoft.com/intune/macos-enroll)和[Windows](https://docs.microsoft.com/intune/windows-enrollment-methods)的註冊設定檔, 都是良好的資源。</span><span class="sxs-lookup"><span data-stu-id="5eca9-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="5eca9-106">**規範原則**: 定義裝置必須遵循的規則和設定, 才能相容。</span><span class="sxs-lookup"><span data-stu-id="5eca9-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="5eca9-107">您也可以使用合規性原則來監視裝置, 並通知使用者不合規性。</span><span class="sxs-lookup"><span data-stu-id="5eca9-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="5eca9-108">開始使用[裝置合規性原則](https://docs.microsoft.com/intune/device-compliance-get-started)。</span><span class="sxs-lookup"><span data-stu-id="5eca9-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="5eca9-109">**條件式存取原則**: 根據您輸入的條件, 協助保護組織資源的安全。</span><span class="sxs-lookup"><span data-stu-id="5eca9-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="5eca9-110">例如, 對於不相容的裝置, 請使用條件式存取限制電子郵件和 SharePoint 的存取。</span><span class="sxs-lookup"><span data-stu-id="5eca9-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="5eca9-111">[有條件存取](https://docs.microsoft.com/intune/conditional-access)和[常用方法來使用條件式存取](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use), 是很好的快速入門資源。</span><span class="sxs-lookup"><span data-stu-id="5eca9-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="5eca9-112">**設定檔**: 管理裝置上的功能和設定, 包括電子郵件設定、新增 WiFi 網路、使用內建範本、控制 IOS 和 macOS 裝置功能等等。</span><span class="sxs-lookup"><span data-stu-id="5eca9-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="5eca9-113">從裝置設定[設定檔](https://docs.microsoft.com/intune/device-profiles)開始。</span><span class="sxs-lookup"><span data-stu-id="5eca9-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="5eca9-114">有説明的連結:</span><span class="sxs-lookup"><span data-stu-id="5eca9-114">Helpful links:</span></span>

- [<span data-ttu-id="5eca9-115">使用 Intune 中的裝置原則和設定檔的常見問題、問題及解決方法</span><span class="sxs-lookup"><span data-stu-id="5eca9-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="5eca9-116">對 Intune 中的原則和設定檔進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="5eca9-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
