---
title: 將電腦上線至適用於端點的 Microsoft Defender 的問題
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901558"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="57201-102">將電腦上線至適用於端點的 Microsoft Defender 的問題</span><span class="sxs-lookup"><span data-stu-id="57201-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="57201-103">您可能會在將電腦上線到 MDE 服務時遇到問題。</span><span class="sxs-lookup"><span data-stu-id="57201-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="57201-104">如果您可以存取使用者的電腦，請遵循這些步驟：</span><span class="sxs-lookup"><span data-stu-id="57201-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="57201-105">下載最新預覽版本的 [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) 診斷工具。</span><span class="sxs-lookup"><span data-stu-id="57201-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="57201-106">以滑鼠右鍵按一下 **MDEClientAnalyzer.cmd**，然後選取 [以系統管理員身分執行]。</span><span class="sxs-lookup"><span data-stu-id="57201-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="57201-107">遵循 **MDEClientAnalyzer.htm** 中建議的任何指導方針。</span><span class="sxs-lookup"><span data-stu-id="57201-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="57201-108">如需更詳細的記錄，請檢閱所建立名為 **MDEClientAnalyzerResult** 的子資料夾。</span><span class="sxs-lookup"><span data-stu-id="57201-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="57201-109">如果需要其他指導方針，請連絡[適用於端點的 Microsoft Defender 支援](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)，並提供產生的 MDEClientAnalyzerResult.zip 檔案進行分析。</span><span class="sxs-lookup"><span data-stu-id="57201-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
