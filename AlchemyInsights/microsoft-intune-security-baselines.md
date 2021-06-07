---
title: 使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783189"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="03bff-102">使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置</span><span class="sxs-lookup"><span data-stu-id="03bff-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="03bff-103">Intune 安全性基準可協助保護使用者和裝置。</span><span class="sxs-lookup"><span data-stu-id="03bff-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="03bff-104">安全性基準 Windows 設定預先設定的群組，用來套用已知的設定群組和相關的安全性小組建議的預設值。</span><span class="sxs-lookup"><span data-stu-id="03bff-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="03bff-105">透過在 Intune 中建立安全性基準設定檔，您可以建立由多個裝置群組原則檔組成的範本。</span><span class="sxs-lookup"><span data-stu-id="03bff-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="03bff-106">當您將安全性基準部署至使用者或裝置群組時，設定會套用至在 Windows 10 或更新版本上執行的裝置。</span><span class="sxs-lookup"><span data-stu-id="03bff-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="03bff-107">例如，Microsoft 行動裝置管理 (MDM) 安全性基準會自動啟用抽取式磁碟磁碟機 BitLocker、需要密碼以解除鎖定裝置，以及停用基本驗證。</span><span class="sxs-lookup"><span data-stu-id="03bff-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="03bff-108">當預設值不適用於您的環境時，您可以自訂基準以套用所需的設定。</span><span class="sxs-lookup"><span data-stu-id="03bff-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="03bff-109">安全性基準也可協助在 Microsoft 365 中建立端對端安全工作流程。</span><span class="sxs-lookup"><span data-stu-id="03bff-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="03bff-110">安全性基準包含影響安全性之設定的最佳作法和建議。</span><span class="sxs-lookup"><span data-stu-id="03bff-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="03bff-111">Intune 合作夥伴使用 Windows 安全小組為群組原則建立基準，所以這些建議是以堅實的指導和廣泛的經驗為基礎。</span><span class="sxs-lookup"><span data-stu-id="03bff-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="03bff-112">如果您是最新的 Intune，且不確定開始位置，安全性基準會協助您快速建立及部署安全的設定檔。</span><span class="sxs-lookup"><span data-stu-id="03bff-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="03bff-113">如果您目前使用群組原則，由於安全性基準已內置於 Intune 中，所以針對管理目的遷移至 Intune 會更容易，並包含切削 edge 的管理功能。</span><span class="sxs-lookup"><span data-stu-id="03bff-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="03bff-114">若要深入瞭解，請參閱[Windows 安全性基準](/windows/security/threat-protection/windows-security-baselines)及行動[裝置管理](/windows/client-management/mdm/)。</span><span class="sxs-lookup"><span data-stu-id="03bff-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

