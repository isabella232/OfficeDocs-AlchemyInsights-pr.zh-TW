---
title: 使用 Microsoft Intune 安全性基準設定 Windows 10 裝置
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571795"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="3816e-102">使用 Microsoft Intune 安全性基準設定 Windows 10 裝置</span><span class="sxs-lookup"><span data-stu-id="3816e-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="3816e-103">Intune 安全性基準可協助保護使用者和裝置。</span><span class="sxs-lookup"><span data-stu-id="3816e-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="3816e-104">安全性基準為 Windows 設定預先設定的群組，用來套用已知的設定群組和相關的安全性小組建議的預設值。</span><span class="sxs-lookup"><span data-stu-id="3816e-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="3816e-105">透過在 Intune 中建立安全性基準設定檔，您可以建立由多個裝置設定設定檔群組成的範本。</span><span class="sxs-lookup"><span data-stu-id="3816e-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="3816e-106">當您將安全性基準部署至使用者或裝置群組時，這些設定會套用至在 Windows 10 或更新版本上執行的裝置。</span><span class="sxs-lookup"><span data-stu-id="3816e-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="3816e-107">例如，MDM 安全性基準會自動 (1) 啟用抽取式磁碟磁碟機 BitLocker， (2) 需要密碼才能解除裝置鎖定，而 (3) 會停用基本驗證。</span><span class="sxs-lookup"><span data-stu-id="3816e-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="3816e-108">當預設值不適用於您的環境時，請自訂基準來套用您所需的設定。</span><span class="sxs-lookup"><span data-stu-id="3816e-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="3816e-109">安全性基準也有助於在 Microsoft 365 中建立端對端的安全工作流程。</span><span class="sxs-lookup"><span data-stu-id="3816e-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="3816e-110">以下是一些優點：</span><span class="sxs-lookup"><span data-stu-id="3816e-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="3816e-111">安全性基準包含影響安全性之設定的最佳作法和建議。</span><span class="sxs-lookup"><span data-stu-id="3816e-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="3816e-112">因為 Intune 與 Windows 安全小組建立群組原則的基準，所以這些建議是以堅實的指導和廣泛的經驗為基礎。</span><span class="sxs-lookup"><span data-stu-id="3816e-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="3816e-113">如果您是最新的 Intune，而且不確定要從何處開始，安全性基準將協助您快速建立及部署安全的設定檔。</span><span class="sxs-lookup"><span data-stu-id="3816e-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="3816e-114">如果您目前使用群組原則，將安全性基準遷移到 Intune 以進行管理，因為它們已內置於 Intune 中，且包含用於管理的前沿功能。</span><span class="sxs-lookup"><span data-stu-id="3816e-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="3816e-115">若要深入瞭解，請參閱 [Windows 安全性基準](https://go.microsoft.com/fwlink/?linkid=2141503) 和行動 [裝置管理](https://go.microsoft.com/fwlink/?linkid=2141701)。</span><span class="sxs-lookup"><span data-stu-id="3816e-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>