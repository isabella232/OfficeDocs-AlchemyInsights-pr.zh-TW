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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826154"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="a0ffc-102">針對 PST 匯入問題進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="a0ffc-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="a0ffc-103">如果您是在 Outlook 用戶端內匯入，請參閱[修正 Outlook .pst 檔案的匯入問題](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。</span><span class="sxs-lookup"><span data-stu-id="a0ffc-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="a0ffc-104">如果您是使用「匯入服務」並發生停滯，請注意，您上傳到 Azure 儲存體位置的每個 PST 檔案都不應超過 20 GB。</span><span class="sxs-lookup"><span data-stu-id="a0ffc-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="a0ffc-105">大於 20 GB 的 PST 檔案可能會影響 PST 匯入程序的效能。</span><span class="sxs-lookup"><span data-stu-id="a0ffc-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="a0ffc-106">如果您想要驗證特定匯入作業的狀態，您可以使用 [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。</span><span class="sxs-lookup"><span data-stu-id="a0ffc-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="a0ffc-107">如需有關匯入服務的完整詳細資料，請參閱[匯入組織 PST 檔案的概觀](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="a0ffc-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
