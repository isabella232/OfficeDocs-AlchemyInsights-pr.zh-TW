---
title: 1336 RecoverableItems 資料夾已滿
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370378"
---
# <a name="the-recoverable-items-folder-is-full"></a>[可復原的專案] 資料夾已滿

對於 Office 365 中的 Exchange Online 信箱, [可復原的專案] 資料夾的預設儲存限制為 30 GB。 如果信箱處於訴訟暫止、eDiscovery 保留或指派給 Office 365 保留原則, 則 [可復原的專案] 資料夾的儲存限制會自動增加至 100 GB。

當 [可復原的專案] 資料夾達到儲存限制時, 信箱功能會受到下列方式的影響:

- 使用者無法刪除信箱中的專案。

- 受管理的資料夾助理無法根據保留標記或受管理的資料夾設定來刪除專案。

- 針對已啟用單一專案復原或處於保留狀態的信箱, 「寫入時複製」頁面保護程式無法維護使用者編輯的專案版本。

- 如果是已啟用信箱審核記錄的信箱, 則 [可復原的專案] 資料夾中的 [audit] 子資料夾中不能儲存任何信箱審核記錄專案。

對於未保留的信箱, 系統管理員可以使用 Exchange `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Online PowerShell 中的命令來刪除 [可復原的專案] 資料夾中的專案。 如需詳細資訊，請參閱下列主題：

- [搜尋並刪除郵件](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [搜尋-信箱](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

對於處於保留狀態的信箱, 系統管理員必須先移除保留, 才能從 [可復原的專案] 資料夾中刪除專案。 如需詳細資訊, 請參閱[刪除雲端式信箱的 [可復原的專案] 資料夾中的專案](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。

為了協助防止 [可復原的專案] 資料夾變滿, 系統管理員可以增加保留信箱的 [可復原的專案] 資料夾的儲存限制, 並設定將 [可復原的專案] 資料夾中的專案移至使用者的封存的信箱保留原則郵件. 請參閱[增加保留信箱的可復原專案配額](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
