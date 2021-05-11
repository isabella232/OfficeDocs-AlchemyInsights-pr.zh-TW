---
title: 針對匯入服務工作停滯問題進行疑難排解
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059841"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="c0de7-102">針對匯入服務工作停滯問題進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="c0de7-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="c0de7-103">如果您遇到匯入服務工作停滯或失敗的問題，請檢查並嘗試下列操作：</span><span class="sxs-lookup"><span data-stu-id="c0de7-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="c0de7-104">檢查 PST 檔案的大小。</span><span class="sxs-lookup"><span data-stu-id="c0de7-104">Review the size of of the PST file.</span></span> <span data-ttu-id="c0de7-105">用於匯入的 PST 檔案的建議大小上限為 20GB。</span><span class="sxs-lookup"><span data-stu-id="c0de7-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="c0de7-106">如果您懷疑略過的項目是因為損毀，請執行 Scanpst.exe 來診斷並修正 PST 檔案中的錯誤。</span><span class="sxs-lookup"><span data-stu-id="c0de7-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="c0de7-107">如果您在匯入期間看到 "MapiExceptionShutoffQuotaExceeded" 錯誤，請確定目標信箱有足夠的容量可匯入所需的 PST 檔案。</span><span class="sxs-lookup"><span data-stu-id="c0de7-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="c0de7-108">如需針對 PST 匯入工作問題進行疑難排解的詳細資訊，請參閱[針對 PST 匯入工作的問題進行疑難排解](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c0de7-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="c0de7-109">如需有關如何修正將 PST 匯入至 Outlook 時的問題的資訊，請參閱[修正匯入 Outlook .pst 檔案時發生的問題 (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us) (機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c0de7-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>