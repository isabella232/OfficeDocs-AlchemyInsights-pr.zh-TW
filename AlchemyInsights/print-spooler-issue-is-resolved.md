---
title: 已解決列印多工緩衝處理器問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083932"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="ae487-102">已解決列印多工緩衝處理器問題</span><span class="sxs-lookup"><span data-stu-id="ae487-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="ae487-103">如果您的裝置更新為 Windows 10 **作業系統組建 19041.329**，您可能會發現特定印表機無法列印的問題。</span><span class="sxs-lookup"><span data-stu-id="ae487-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="ae487-104">列印多工緩衝處理器可能會在嘗試列印時發生錯誤或意外關閉，且受影響的印表機不會有任何輸出。</span><span class="sxs-lookup"><span data-stu-id="ae487-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="ae487-105">此問題已在作業系統組建 **19041.331**、[KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523) 中解決。</span><span class="sxs-lookup"><span data-stu-id="ae487-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="ae487-106">**持續調查**</span><span class="sxs-lookup"><span data-stu-id="ae487-106">**Ongoing investigation**</span></span>

<span data-ttu-id="ae487-107">在部分裝置上，本機安全性授權子系統服務 (LSASS) 檔案 (**Isass.exe**) 可能會失敗，並顯示以下錯誤訊息：「重要系統處理序 C:\WINDOWS\system32\Isass.exe 失敗，狀態碼為 c0000008。</span><span class="sxs-lookup"><span data-stu-id="ae487-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="ae487-108">電腦現在必須重新開機」。</span><span class="sxs-lookup"><span data-stu-id="ae487-108">The machine must now be restarted".</span></span>  <span data-ttu-id="ae487-109">**Microsoft 正努力研究解決方法，並會在即將推出的版本中提供更新。**</span><span class="sxs-lookup"><span data-stu-id="ae487-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="ae487-110">如需詳細資訊，請參閱 [Windows 10 版本 2004 已知問題](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)。</span><span class="sxs-lookup"><span data-stu-id="ae487-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>