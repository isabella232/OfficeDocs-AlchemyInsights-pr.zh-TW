---
title: 電腦上線的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676873"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="0d9ac-102">電腦上線的問題</span><span class="sxs-lookup"><span data-stu-id="0d9ac-102">Issues with onboarding machines</span></span>

<span data-ttu-id="0d9ac-103">將電腦上線到 MDATP 服務時，您可能會遇到問題。</span><span class="sxs-lookup"><span data-stu-id="0d9ac-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="0d9ac-104">若您想要存取終端使用者的電腦，請依照下列步驟操作：</span><span class="sxs-lookup"><span data-stu-id="0d9ac-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="0d9ac-105">下載 [用戶端連線分析程式](https://aka.ms/mdatpanalyzer) 診斷工具。</span><span class="sxs-lookup"><span data-stu-id="0d9ac-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="0d9ac-106">解壓縮並執行 MDATPAnalyzer.cmd 指令。</span><span class="sxs-lookup"><span data-stu-id="0d9ac-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="0d9ac-107">在名為 MDATPClientAnalyzerResult 的資料夾（用於下載分析器工具的同個資料夾 ）中找到 [診斷記錄]。</span><span class="sxs-lookup"><span data-stu-id="0d9ac-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="0d9ac-108">檢視記錄檔 MDATPClientAnalyzer.txt 並用以查找連線或網際網路 proxy 設定問題。</span><span class="sxs-lookup"><span data-stu-id="0d9ac-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>