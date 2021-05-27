---
title: 受攻擊面縮小規則
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651478"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="25f9a-102">受攻擊面縮小規則</span><span class="sxs-lookup"><span data-stu-id="25f9a-102">Attack surface reduction rules</span></span>

<span data-ttu-id="25f9a-103">排除檔案或資料夾可能會嚴重降低受攻擊面縮小規則所提供的保護。</span><span class="sxs-lookup"><span data-stu-id="25f9a-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="25f9a-104">允許執行規則所封鎖的檔案，而且不會記錄任何報告或事件。</span><span class="sxs-lookup"><span data-stu-id="25f9a-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="25f9a-105">排除會套用到允許排除的所有規則。</span><span class="sxs-lookup"><span data-stu-id="25f9a-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="25f9a-106">ASR 排除會使用與 Microsoft Defender 防毒軟體排除相同的語法。</span><span class="sxs-lookup"><span data-stu-id="25f9a-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="25f9a-107">如需詳細資料，請參閱[設定及驗證 Microsoft Defender 防毒軟體掃描的排除項目](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="25f9a-108">若要避免問題，請檢閱[定義排除時應避免的常見錯誤](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="25f9a-109">並非所有 ASR 規則都支援排除。</span><span class="sxs-lookup"><span data-stu-id="25f9a-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="25f9a-110">若要驗證您的規則是否支援排除，請參閱[受攻擊面縮小規則](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)表格。</span><span class="sxs-lookup"><span data-stu-id="25f9a-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="25f9a-111">受攻擊面縮小規則</span><span class="sxs-lookup"><span data-stu-id="25f9a-111">Attack surface reduction rules</span></span>

<span data-ttu-id="25f9a-112">您的組織受攻擊面包括攻擊者可能會危害組織裝置或網路的所有位置。</span><span class="sxs-lookup"><span data-stu-id="25f9a-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="25f9a-113">減少受攻擊面表示保護組織裝置和網路，減少攻擊者執行攻擊的方式。</span><span class="sxs-lookup"><span data-stu-id="25f9a-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="25f9a-114">在適用於端點的 Microsoft Defender 中設定受攻擊面縮小規則可以有所幫助。</span><span class="sxs-lookup"><span data-stu-id="25f9a-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="25f9a-115">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="25f9a-115">For more information, see:</span></span>

- [<span data-ttu-id="25f9a-116">將 ASR 規則 GUID 對應到名稱</span><span class="sxs-lookup"><span data-stu-id="25f9a-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="25f9a-117">ASR 規則需求：</span><span class="sxs-lookup"><span data-stu-id="25f9a-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="25f9a-118">Windows 10 專業版，版本 1709 或更新版本</span><span class="sxs-lookup"><span data-stu-id="25f9a-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="25f9a-119">Windows 10 企業版，版本 1709 或更新版本</span><span class="sxs-lookup"><span data-stu-id="25f9a-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="25f9a-120">Windows Server 版本 1803 (半年通道) 或更新版本</span><span class="sxs-lookup"><span data-stu-id="25f9a-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="25f9a-121">識別要套用的正確排除</span><span class="sxs-lookup"><span data-stu-id="25f9a-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="25f9a-122">在 Microsoft-Windows-Windows Defender/Operational 記錄中尋找 eventID 1121 或 1122。</span><span class="sxs-lookup"><span data-stu-id="25f9a-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="25f9a-123">評估區塊案例和內容，並確認此案例需要取消封鎖。</span><span class="sxs-lookup"><span data-stu-id="25f9a-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="25f9a-124">讀取事件詳細資料中的 Path 值，這是定義排除的值。</span><span class="sxs-lookup"><span data-stu-id="25f9a-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="25f9a-125">盡可能設定嚴格的排除。</span><span class="sxs-lookup"><span data-stu-id="25f9a-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="25f9a-126">視需要套用萬用字元 (例如，取代 User 變數)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="25f9a-127">根據部署需求套用排除。</span><span class="sxs-lookup"><span data-stu-id="25f9a-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="25f9a-128">如需詳細資料，請參閱[自訂受攻擊面縮小規則](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="25f9a-129">未遵守排除</span><span class="sxs-lookup"><span data-stu-id="25f9a-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="25f9a-130">判斷規則是否支援排除。</span><span class="sxs-lookup"><span data-stu-id="25f9a-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="25f9a-131">如需詳細資料，請參閱[受攻擊面縮小規則](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="25f9a-132">檢閱套用的排除，並驗證事件資料是否包含錯字或解譯錯誤的萬用字元。</span><span class="sxs-lookup"><span data-stu-id="25f9a-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="25f9a-133">如需詳細資訊，請參閱[支援的排除類型](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="25f9a-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="25f9a-134">如果規則的影響太高，請考慮將規則移到 (移回) 稽核模式，以執行進一步的驗證。</span><span class="sxs-lookup"><span data-stu-id="25f9a-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="25f9a-135">如需詳細資料，請參閱[測試適用於端點的 Microsoft Defender 功能在稽核模式中的運作方式](/microsoft-365/security/defender-endpoint/audit-windows-defender) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="25f9a-136">使用此命令收集支援資料以開啟支援案例：</span><span class="sxs-lookup"><span data-stu-id="25f9a-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="25f9a-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="25f9a-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="25f9a-138">如需詳細資訊，請參閱[將電腦上線至適用於端點的 Microsoft Defender 的問題](issues-with-onboarding-machines.md)。</span><span class="sxs-lookup"><span data-stu-id="25f9a-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
