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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657920"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="e13f8-102">設定端點 DLP</span><span class="sxs-lookup"><span data-stu-id="e13f8-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="e13f8-103">Microsoft 端點 DLP 可讓可以您將 DLP 保護和監視功能延伸到 Windows 10 裝置上的敏感性資訊。</span><span class="sxs-lookup"><span data-stu-id="e13f8-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="e13f8-104">將裝置上線至裝置管理中後，您就可以建立 DLP 原則，在項目上強制執行保護動作。</span><span class="sxs-lookup"><span data-stu-id="e13f8-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="e13f8-105">活動總管可用來監視敏感性項目的活動。</span><span class="sxs-lookup"><span data-stu-id="e13f8-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="e13f8-106">如需詳細資訊，請參閱 [將裝置上線至裝置管理](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="e13f8-107">若要開始使用端點 DLP：</span><span class="sxs-lookup"><span data-stu-id="e13f8-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="e13f8-108">請確認您擁有適當的 SKU/訂閱授權。</span><span class="sxs-lookup"><span data-stu-id="e13f8-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="e13f8-109">如需詳細資訊，請參閱 [SKU/訂閱授權](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="e13f8-p103">檢查啟用裝置管理、存取上線頁面或開啟/關閉裝置監視所需的權限。如需詳細資訊，請參閱[權限](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="e13f8-112">遵循上線裝置程序將裝置上線至裝置管理。</span><span class="sxs-lookup"><span data-stu-id="e13f8-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="e13f8-113">如需詳細資訊，請參閱 [上線裝置](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="e13f8-114">建立 DLP 原則以保護您的敏感性項目。</span><span class="sxs-lookup"><span data-stu-id="e13f8-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="e13f8-115">如需詳細資訊，請參閱 [端點 DLP 原則案例](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="e13f8-116">如需有關 Microsoft 端點 DLP，請參閱 [深入了解 Microsoft 365 端點資料外洩防護 (預覽版)](/microsoft-365/compliance/endpoint-dlp-learn-about)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="e13f8-117">**如果需要支援，以下是重要資料收集步驟：**</span><span class="sxs-lookup"><span data-stu-id="e13f8-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="e13f8-118">下載 [MDATP 用戶端分析器預覽](https://aka.ms/betamdatpanalyzer)。</span><span class="sxs-lookup"><span data-stu-id="e13f8-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="e13f8-119">使用 cmd 視窗以系統管理員身分執行工具：</span><span class="sxs-lookup"><span data-stu-id="e13f8-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="e13f8-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="e13f8-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="e13f8-121">當系統提示 [輸入收集追蹤的分鐘數:] 時，輸入執行案例所需的分鐘數。</span><span class="sxs-lookup"><span data-stu-id="e13f8-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="e13f8-122">執行案例。</span><span class="sxs-lookup"><span data-stu-id="e13f8-122">Run the scenario.</span></span>

<span data-ttu-id="e13f8-123">收集 Zip 檔案輸出，以提供給支援專員。</span><span class="sxs-lookup"><span data-stu-id="e13f8-123">Collect the Zip file output to give to the Support agent.</span></span>
