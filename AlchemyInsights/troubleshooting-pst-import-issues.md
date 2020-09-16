---
title: 針對 PST 匯入問題進行疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5fdb713f321e5c9f67a6078739c31a90571b913d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757731"
---
# <a name="troubleshooting-pst-import-issues"></a>針對 PST 匯入問題進行疑難排解

- 如果您是在 Outlook 用戶端內匯入，請參閱[修正 Outlook .pst 檔案的匯入問題](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。

- 如果您是使用「匯入服務」並發生停滯，請注意，您上傳到 Azure 儲存體位置的每個 PST 檔案都不應超過 20 GB。 大於 20 GB 的 PST 檔案可能會影響 PST 匯入程序的效能。

- 如果您想要驗證特定匯入作業的狀態，您可以使用 [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。

- 如需有關匯入服務的完整詳細資料，請參閱[匯入組織 PST 檔案的概觀](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。
