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
ms.openlocfilehash: bf07102d01d85eaed8ea95b571a0eabea7c4b7448839294f37e5e30134e04282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105091"
---
# <a name="troubleshooting-import-service-job-stuck"></a>針對匯入服務工作停滯問題進行疑難排解

如果您遇到匯入服務工作停滯或失敗的問題，請檢查並嘗試下列操作：

- 檢查 PST 檔案的大小。 用於匯入的 PST 檔案的建議大小上限為 20GB。

- 如果您懷疑略過的項目是因為損毀，請執行 Scanpst.exe 來診斷並修正 PST 檔案中的錯誤。

- 如果您在匯入期間看到 "MapiExceptionShutoffQuotaExceeded" 錯誤，請確定目標信箱有足夠的容量可匯入所需的 PST 檔案。

如需針對 PST 匯入工作問題進行疑難排解的詳細資訊，請參閱[針對 PST 匯入工作的問題進行疑難排解](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job) (部分機器翻譯)。

如需有關如何修正將 PST 匯入至 Outlook 時的問題的資訊，請參閱[修正匯入 Outlook .pst 檔案時發生的問題 (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us) (機器翻譯)。