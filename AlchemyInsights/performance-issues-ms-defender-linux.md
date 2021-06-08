---
title: Linux 上適用於端點的 Microsoft Defender 效能問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783422"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="030df-102">Linux 上適用於端點的 Microsoft Defender 效能問題</span><span class="sxs-lookup"><span data-stu-id="030df-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="030df-103">本文引導您完成識別 Linux 上適用於端點的 Microsoft Defender 效能問題的步驟。</span><span class="sxs-lookup"><span data-stu-id="030df-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="030df-104">重要的是，要先驗證您遇到的問題是使用 [最新版本](/microsoft-365/security/defender-endpoint/linux-whatsnew) 解決的。</span><span class="sxs-lookup"><span data-stu-id="030df-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="030df-105">若要啟動您的調查，請參閱 [疑難排解 Linux 上適用於端點的 Microsoft Defender 效能問題](/microsoft-365/security/defender-endpoint/linux-support-perf)。</span><span class="sxs-lookup"><span data-stu-id="030df-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="030df-106">排除項目</span><span class="sxs-lookup"><span data-stu-id="030df-106">Exclusions</span></span>

<span data-ttu-id="030df-107">排除項目可以協助降低效能問題。</span><span class="sxs-lookup"><span data-stu-id="030df-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="030df-108">在您開始之前先檢視您的排除項目，以得知任何其他風險並紀錄之。</span><span class="sxs-lookup"><span data-stu-id="030df-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="030df-109">如需詳細資訊，請參閱[設定及驗證 Linux 上適用於端點的 Microsoft Defender 排除項目](/microsoft-365/security/defender-endpoint/linux-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="030df-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="030df-110">當您有多個位於相同掛接點的檔案和資料夾要進行排除時，在掛接點進行排除可能更為容易。</span><span class="sxs-lookup"><span data-stu-id="030df-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="030df-111">從二月份發行版本 101.22.80 開始，您可以排除整個掛接點。</span><span class="sxs-lookup"><span data-stu-id="030df-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="030df-112">例如，如果 /mnt/backup 是一個掛接點，您可以透過執行此命令，將 /mnt/backup 新增至排除清單：</span><span class="sxs-lookup"><span data-stu-id="030df-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="030df-113">**注意**：新增排除項目會增加無法偵測的惡意程式碼風險，且應小心處置和執行。</span><span class="sxs-lookup"><span data-stu-id="030df-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="030df-114">需要協助嗎？</span><span class="sxs-lookup"><span data-stu-id="030df-114">Need Help?</span></span>

<span data-ttu-id="030df-115">若要以最有效的方式協助您，請在開啟支援案例之前，收集診斷資料。</span><span class="sxs-lookup"><span data-stu-id="030df-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
