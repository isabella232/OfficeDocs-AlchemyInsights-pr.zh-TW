---
title: 針對 PST 匯入問題進行疑難排解
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059806"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="23803-102">針對 PST 匯入問題進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="23803-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="23803-103">如果您是在 Outlook 用戶端內匯入，請參閱[修正 Outlook .pst 檔案的匯入問題](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。</span><span class="sxs-lookup"><span data-stu-id="23803-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="23803-104">如果您是使用「匯入服務」並發生停滯，請注意，您上傳到 Azure 儲存體位置的每個 PST 檔案都不應超過 20GB。</span><span class="sxs-lookup"><span data-stu-id="23803-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="23803-105">大於 20GB 的 PST 檔案可能會影響 PST 匯入程序的效能。</span><span class="sxs-lookup"><span data-stu-id="23803-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="23803-106">如需疑難排解停滯工作的詳細資訊，請參閱[會影響 PST 匯入工作的問題](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)。</span><span class="sxs-lookup"><span data-stu-id="23803-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="23803-107">如果您想要驗證特定匯入工作的狀態，請使用 [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。</span><span class="sxs-lookup"><span data-stu-id="23803-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="23803-108">如需有關匯入服務的完整詳細資料，請參閱[匯入組織 PST 檔案的概觀](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="23803-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
