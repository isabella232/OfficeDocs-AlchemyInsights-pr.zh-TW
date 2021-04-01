---
title: 端點管理員 - 安全性基準
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440868"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="6ebb2-102">端點管理員 - 安全性基準</span><span class="sxs-lookup"><span data-stu-id="6ebb2-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="6ebb2-103">安全性基準是預先設定的 Windows 設定群組，可協助您套用相關安全小組建議的安全性設定。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="6ebb2-104">您可以自訂這些基準，以只提供所需的設定和值。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="6ebb2-105">如需安全性基準的詳細資訊，請參閱[在 Intune 中使用安全性基準來設定 Windows 10 裝置](https://docs.microsoft.com/mem/intune/protect/security-baselines)。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="6ebb2-106">這些產品目前有基準：</span><span class="sxs-lookup"><span data-stu-id="6ebb2-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="6ebb2-107">Windows MDM 安全性設定</span><span class="sxs-lookup"><span data-stu-id="6ebb2-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="6ebb2-108">適用於端點的 Microsoft Defender 安全性</span><span class="sxs-lookup"><span data-stu-id="6ebb2-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="6ebb2-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6ebb2-109">Microsoft Edge</span></span>

<span data-ttu-id="6ebb2-110">每個基準會定期更新，並且以增量版本形式發行。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="6ebb2-111">每個版本會新增或移除舊版的設定，以確保該基準符合目前的指導方針。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="6ebb2-112">端點安全性中的安全性基準主控台透過讓不同版本的變更可顯示，以比較不同的版本。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="6ebb2-113">如需如何最有效地變更所部署基準版本的指引，請參閱[在 Microsoft Intune 中管理安全性基準設定檔](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="6ebb2-114">部署安全性基準之後，您可以監視部署狀態，並依據裝置檢查設定。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="6ebb2-115">**注意：** 從初始部署到裝置可能需要最多 24 小時才能顯示比較基準的報告資料，且可能需要 6 小時，才能取得進一步的更新。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="6ebb2-116">基準設定不適用最常見的原因是在已在不同的設定檔中使用相同的設定。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="6ebb2-117">您可以在安全性基準設定檔的 [裝置狀態] 節點內選取裝置，以調查特定裝置的狀況。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="6ebb2-118">如需詳細資料，請參閱[解決安全性基準的衝突](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)。</span><span class="sxs-lookup"><span data-stu-id="6ebb2-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>