---
title: 疑難排解電子文件探索保留錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583750"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="42def-102">疑難排解電子文件探索保留錯誤</span><span class="sxs-lookup"><span data-stu-id="42def-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="42def-103">發生電子文件探索保留問題嗎？</span><span class="sxs-lookup"><span data-stu-id="42def-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="42def-104">以下是可考慮的一些最佳做法：</span><span class="sxs-lookup"><span data-stu-id="42def-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="42def-105">檢查保留發佈狀態。</span><span class="sxs-lookup"><span data-stu-id="42def-105">Check the hold distribution status.</span></span>  <span data-ttu-id="42def-106">若狀態為 **開啟 (擱置中)** 或 **關閉 (擱置中)**，請等候保留發布完成。</span><span class="sxs-lookup"><span data-stu-id="42def-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="42def-107">將電子文件探索保留更新合併入單一大量要求，而非重複地為每次交易更新此原則。</span><span class="sxs-lookup"><span data-stu-id="42def-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="42def-108">在安全性和合規性中心 PowerShell 中執行 Set-CaseHoldPolicy <policyname> -RetryDistribution。</span><span class="sxs-lookup"><span data-stu-id="42def-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="42def-109">如需詳細資料，請參閱 [連線到安全性和合規性中心 PowerShel](/powershell/exchange/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="42def-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="42def-110">如需緩解及解決電子文件探索保留問題的檢查設定和其它最佳做法的步驟，請參閱 [疑難排解電子文件探索保留錯誤](/microsoft-365/compliance/hold-distribution-errors)。</span><span class="sxs-lookup"><span data-stu-id="42def-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="42def-111">如需有關疑難排解其它常見電子文件探索問題的資訊，請參閱 [調查、疑難排解和解決常見電子文件探索問題](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)。</span><span class="sxs-lookup"><span data-stu-id="42def-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
