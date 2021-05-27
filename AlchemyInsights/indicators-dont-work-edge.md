---
title: 使用 Edge 瀏覽器時，指示器無法運作
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651490"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="b54e8-102">使用 Edge 瀏覽器時，指示器無法運作</span><span class="sxs-lookup"><span data-stu-id="b54e8-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="b54e8-103">建立指示器之後，Edge (Smartscreen) 不使用該指示器。</span><span class="sxs-lookup"><span data-stu-id="b54e8-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="b54e8-104">如需詳細資訊，請參閱[為 IP 和 URL/網域建立指示器](/microsoft-365/security/defender-endpoint/indicator-ip-domain) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="b54e8-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="b54e8-105">步驟 1：確定下列項目</span><span class="sxs-lookup"><span data-stu-id="b54e8-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="b54e8-106">確定指示器正確 (IP/URL 沒有錯字、動作正確、RBAC 群組正確)。</span><span class="sxs-lookup"><span data-stu-id="b54e8-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="b54e8-107">建立指示器後至少等待 2 小時，以考慮到任何可能的延遲。</span><span class="sxs-lookup"><span data-stu-id="b54e8-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="b54e8-108">確認系統已上線至適用於端點的 Microsoft Defender。</span><span class="sxs-lookup"><span data-stu-id="b54e8-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="b54e8-109">確認系統可與雲端通訊。</span><span class="sxs-lookup"><span data-stu-id="b54e8-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="b54e8-110">請至[測試網站](https://demo.smartscreen.msft.net)頁面，確認 Smartscreen 已啟用並可連線。</span><span class="sxs-lookup"><span data-stu-id="b54e8-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="b54e8-111">步驟 2：疑難排解可能的問題</span><span class="sxs-lookup"><span data-stu-id="b54e8-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="b54e8-112">確定用戶端符合需求。</span><span class="sxs-lookup"><span data-stu-id="b54e8-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="b54e8-113">如需詳細資料，請參閱[為 IP 和 URL/網域建立指示器](/microsoft-365/security/defender-endpoint/indicator-ip-domain) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="b54e8-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="b54e8-114">確定您執行的是最新版的 Edge 瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="b54e8-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="b54e8-115">若要了解最新版本，請參閱[了解您所擁有的 Microsoft Edge 版本](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)。</span><span class="sxs-lookup"><span data-stu-id="b54e8-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="b54e8-116">重新啟動 Edge 瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="b54e8-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="b54e8-117">瀏覽至已設定指示器的網站。</span><span class="sxs-lookup"><span data-stu-id="b54e8-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="b54e8-118">如果網站未如預期顯示，請繼續執行步驟 3。</span><span class="sxs-lookup"><span data-stu-id="b54e8-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="b54e8-119">步驟 3：收集資料</span><span class="sxs-lookup"><span data-stu-id="b54e8-119">Step 3: Collect data</span></span>

- <span data-ttu-id="b54e8-120">收集 **MDEClientAnalyzer** 診斷資料。</span><span class="sxs-lookup"><span data-stu-id="b54e8-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="b54e8-121">如需指示，請參閱[將電腦上線至適用於端點的 Microsoft Defender 的問題](issues-with-onboarding-machines.md)。</span><span class="sxs-lookup"><span data-stu-id="b54e8-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="b54e8-122">如果您願意安裝及收集 Fiddler 追蹤，請參閱 [Telerik Fiddler](http://www.telerik.com/fiddler)。</span><span class="sxs-lookup"><span data-stu-id="b54e8-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="b54e8-123">如果您想獲得 Microsoft 支援服務的指引，請選取下方的 [支援] 圖示以開啟支援案例。</span><span class="sxs-lookup"><span data-stu-id="b54e8-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
