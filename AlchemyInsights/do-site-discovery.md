---
title: 執行網站探索
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529193"
---
# <a name="do-site-discovery"></a><span data-ttu-id="e5f09-102">執行網站探索</span><span class="sxs-lookup"><span data-stu-id="e5f09-102">Do site discovery</span></span>

<span data-ttu-id="e5f09-103">如果組織仍使用舊版 Web 應用程式並計劃來使用 Internet Explorer 模式 (大部分客戶會這麼做)，則您應該執行一些額外的網站探索。</span><span class="sxs-lookup"><span data-stu-id="e5f09-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="e5f09-104">**您已部署舊版 Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="e5f09-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="e5f09-105">如果您已經將企業網站清單設定為可對舊版 Microsoft Edge 運作，則您的網站探索幾乎已完成。</span><span class="sxs-lookup"><span data-stu-id="e5f09-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="e5f09-106">您可能需要做的一件事是新增中性網站。</span><span class="sxs-lookup"><span data-stu-id="e5f09-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="e5f09-107">中性網站通常是提供單一登入 (SSO) 的網站。</span><span class="sxs-lookup"><span data-stu-id="e5f09-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="e5f09-108">如果您從 Microsoft Edge 前往中性網站，則您會想要保持在 Microsoft Edge 中以進行驗證。</span><span class="sxs-lookup"><span data-stu-id="e5f09-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="e5f09-109">如果您以 Internet Explorer 模式前往中性網站，則您會想要保持 Internet Explorer 模式中以進行驗證。</span><span class="sxs-lookup"><span data-stu-id="e5f09-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="e5f09-110">識別您使用的任何 SSO 或其他中性網站，並將其新增到您的企業網站清單。</span><span class="sxs-lookup"><span data-stu-id="e5f09-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="e5f09-111">**Internet Explorer 是您的預設瀏覽器**</span><span class="sxs-lookup"><span data-stu-id="e5f09-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="e5f09-112">如果您現在僅使用 Internet Explorer，可能不知道哪些網站已升級至新式 Web 標準，以及哪些網站仍需要 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="e5f09-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="e5f09-113">您將需要尋找並將這些網站新增到企業網站清單，以便可以只針對這些網站使用 Internet Explorer 模式。</span><span class="sxs-lookup"><span data-stu-id="e5f09-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="e5f09-114">[企業網站探索](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery)會探索可能需要 Internet Explorer 模式的網站。</span><span class="sxs-lookup"><span data-stu-id="e5f09-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="e5f09-115">它可以在 Windows 10、Windows 8.1 或 Windows 7 上從執行 Internet Explorer 8 到 Internet Explorer 11 的電腦上收集資料。</span><span class="sxs-lookup"><span data-stu-id="e5f09-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="e5f09-116">**分析資料**</span><span class="sxs-lookup"><span data-stu-id="e5f09-116">**Analyze the data**</span></span>

<span data-ttu-id="e5f09-117">收集網站資料之後，建議您執行下列的四個步驟程序來分析資料：</span><span class="sxs-lookup"><span data-stu-id="e5f09-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="e5f09-118">依網域然後依 URL 排序資料。</span><span class="sxs-lookup"><span data-stu-id="e5f09-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="e5f09-119">定義要針對 Internet Explorer 模式設定的應用程式界限。</span><span class="sxs-lookup"><span data-stu-id="e5f09-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="e5f09-120">您想要包含定義應用程式的所有網站和 Web 控制項，但不想包含額外的網站和控制項。</span><span class="sxs-lookup"><span data-stu-id="e5f09-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="e5f09-121">有些網站可能簡單的如 *https://contoso.com/app1* 一般，而其他網站可能需要您定義多個網站和頁面。</span><span class="sxs-lookup"><span data-stu-id="e5f09-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="e5f09-122">測試應用程式以確認它無法原生地運作。</span><span class="sxs-lookup"><span data-stu-id="e5f09-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="e5f09-123">許多網站在偵測新式瀏覽器時會提供新式內容，並且會在偵測到 Internet Explorer 時僅提供舊版內容。</span><span class="sxs-lookup"><span data-stu-id="e5f09-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="e5f09-124">如果應用程式無法通過測試，請將其新增到企業網站清單。</span><span class="sxs-lookup"><span data-stu-id="e5f09-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="e5f09-125">最佳做法是將組成應用程式的所有網站分組。</span><span class="sxs-lookup"><span data-stu-id="e5f09-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="e5f09-126">如此一來，當您升級應用程式時，要從 Internet Explorer 模式移除整個網站，並開始對該應用程式使用新式瀏覽器會比較容易。</span><span class="sxs-lookup"><span data-stu-id="e5f09-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="e5f09-127">完成網站探索並分析資料之後，就可以開始查看您的通道策略。</span><span class="sxs-lookup"><span data-stu-id="e5f09-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

