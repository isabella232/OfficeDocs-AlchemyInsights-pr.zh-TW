---
title: 使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641616"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="ac798-102">使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置</span><span class="sxs-lookup"><span data-stu-id="ac798-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="ac798-103">Intune 安全性基準可協助保護使用者和裝置。</span><span class="sxs-lookup"><span data-stu-id="ac798-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ac798-104">安全性基準是 Windows 設定的預先設定群組，用來套用相關安全小組建議的已知設定群組和預設值。</span><span class="sxs-lookup"><span data-stu-id="ac798-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ac798-105">透過在 Intune 中建立安全性基準設定檔，您可以建立由多個裝置群組原則檔組成的範本。</span><span class="sxs-lookup"><span data-stu-id="ac798-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ac798-106">當您將安全性基準部署至使用者或裝置群組時，這些設定會套用於在 Windows 10 或更新版本上執行的裝置。</span><span class="sxs-lookup"><span data-stu-id="ac798-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="ac798-107">例如，Microsoft 行動裝置管理 (MDM) 安全性基準會自動 (1) 啟用抽取式磁碟機的 BitLocker、(2) 需要密碼才能解除鎖定裝置，以及 (3) 停用基本驗證。</span><span class="sxs-lookup"><span data-stu-id="ac798-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ac798-108">當預設值不適用於您的環境時，您可以自訂基準以套用所需的設定。</span><span class="sxs-lookup"><span data-stu-id="ac798-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ac798-109">安全性基準也可協助在 Microsoft 365 中建立端對端安全工作流程。</span><span class="sxs-lookup"><span data-stu-id="ac798-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ac798-110">以下是此功能的一些益處：</span><span class="sxs-lookup"><span data-stu-id="ac798-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="ac798-111">安全性基準包含影響安全性之設定的最佳作法和建議。</span><span class="sxs-lookup"><span data-stu-id="ac798-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ac798-112">由於 Intune 與建立群組原則基準的 Windows 安全性小組合作，因此這些建議是以可靠的指引和廣泛的經驗為基礎。</span><span class="sxs-lookup"><span data-stu-id="ac798-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ac798-113">如果您第一次使用 Intune 且不確定從何處開始，則安全性基準將可協助快速建立及部署安全的設定檔。</span><span class="sxs-lookup"><span data-stu-id="ac798-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ac798-114">如果您目前正使用群組原則，則搭配安全性基準移入 Intune 來用於管理目的會更容易，因為這些安全性基準內建在 Intune 中，並包含用於管理的最先進功能。</span><span class="sxs-lookup"><span data-stu-id="ac798-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ac798-115">如需詳細資訊，請參閱 [Windows 安全性基準](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)以及[行動裝置管理](https://docs.microsoft.com/windows/client-management/mdm/)。</span><span class="sxs-lookup"><span data-stu-id="ac798-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>