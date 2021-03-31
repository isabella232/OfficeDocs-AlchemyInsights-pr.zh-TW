---
title: 設定端點 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402405"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="fcf31-102">設定端點 DLP</span><span class="sxs-lookup"><span data-stu-id="fcf31-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="fcf31-103">Microsoft 端點 DLP 可讓可以您將 DLP 保護和監視功能延伸到 Windows 10 裝置上的敏感性資訊。</span><span class="sxs-lookup"><span data-stu-id="fcf31-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="fcf31-104">將裝置上線至裝置管理中後，您就可以建立 DLP 原則，在項目上強制執行保護動作。</span><span class="sxs-lookup"><span data-stu-id="fcf31-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="fcf31-105">活動總管可用來監視敏感性項目的活動。</span><span class="sxs-lookup"><span data-stu-id="fcf31-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="fcf31-106">如需詳細資訊，請參閱 [將裝置上線至裝置管理](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。</span><span class="sxs-lookup"><span data-stu-id="fcf31-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="fcf31-107">若要開始使用端點 DLP：</span><span class="sxs-lookup"><span data-stu-id="fcf31-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="fcf31-108">請確認您擁有適當的 SKU/訂閱授權。</span><span class="sxs-lookup"><span data-stu-id="fcf31-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="fcf31-109">如需詳細資訊，請參閱 [SKU/訂閱授權](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。</span><span class="sxs-lookup"><span data-stu-id="fcf31-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="fcf31-110">檢查啟用裝置管理、存取上線頁面或開啟/關閉裝置監視所需的權限。</span><span class="sxs-lookup"><span data-stu-id="fcf31-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="fcf31-111">如需詳細資訊，請參閱 [權限](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。</span><span class="sxs-lookup"><span data-stu-id="fcf31-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="fcf31-112">遵循上線裝置程序將裝置上線至裝置管理。</span><span class="sxs-lookup"><span data-stu-id="fcf31-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="fcf31-113">如果您在 M365 合規性 **設定** 下方找不到 [裝置上線] (預覽) 選項，請確認您擁有上述的適當授權和權限。</span><span class="sxs-lookup"><span data-stu-id="fcf31-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="fcf31-114">如需詳細資訊，請參閱 [上線裝置](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。</span><span class="sxs-lookup"><span data-stu-id="fcf31-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="fcf31-115">建立 DLP 原則以保護您的敏感性項目。</span><span class="sxs-lookup"><span data-stu-id="fcf31-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="fcf31-116">如需詳細資訊，請參閱 [端點 DLP 原則案例](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="fcf31-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="fcf31-117">如需有關 Microsoft 端點 DLP，請參閱 [深入了解 Microsoft 365 端點資料外洩防護 (預覽版)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about)。</span><span class="sxs-lookup"><span data-stu-id="fcf31-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="fcf31-118">**如果需要支援，以下是重要資料收集步驟：**</span><span class="sxs-lookup"><span data-stu-id="fcf31-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="fcf31-119">從 [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer") 下載 MDATP 用戶端分析器預覽</span><span class="sxs-lookup"><span data-stu-id="fcf31-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="fcf31-120">使用 cmd 視窗以系統管理員身分執行工具：</span><span class="sxs-lookup"><span data-stu-id="fcf31-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="fcf31-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="fcf31-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="fcf31-122">當系統出現「輸入收集追蹤的分鐘數：」的提示時，輸入執行案例所需的分鐘數</span><span class="sxs-lookup"><span data-stu-id="fcf31-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="fcf31-123">執行案例</span><span class="sxs-lookup"><span data-stu-id="fcf31-123">Run the scenario</span></span>

<span data-ttu-id="fcf31-124">收集可供支援專員使用的 Zip 檔案輸出。</span><span class="sxs-lookup"><span data-stu-id="fcf31-124">Collect the Zip file output to be given to the Support agent.</span></span>
