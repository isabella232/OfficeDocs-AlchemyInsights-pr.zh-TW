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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972410"
---
# <a name="troubleshooting-pst-import-issues"></a>針對 PST 匯入問題進行疑難排解

- 如果您是在 Outlook 用戶端內匯入，請參閱[修正 Outlook .pst 檔案的匯入問題](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。

- 如果您是使用「匯入服務」並發生停滯，請注意，您上傳到 Azure 儲存體位置的每個 PST 檔案都不應超過 20GB。 大於 20GB 的 PST 檔案可能會影響 PST 匯入程序的效能。 如需疑難排解停滯工作的詳細資訊，請參閱[會影響 PST 匯入工作的問題](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)。

- 如果您想要驗證特定匯入工作的狀態，請使用 [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)。

- 如需有關匯入服務的完整詳細資料，請參閱[匯入組織 PST 檔案的概觀](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)。
