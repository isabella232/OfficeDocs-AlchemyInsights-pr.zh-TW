---
title: 1336 RecoverableItems 資料夾已滿
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061747"
---
# <a name="the-recoverable-items-folder-is-full"></a>[可復原的專案] 資料夾已滿

若為 Exchange Online 信箱，[可復原的專案] 資料夾的預設儲存限制為 30 GB。 如果信箱處於訴訟暫止、eDiscovery 保留或指派給保留原則，則 [可復原的專案] 資料夾的儲存量限制會自動增加至 100 GB。

當 [可復原的專案] 資料夾達到儲存限制時，信箱功能會受到下列方式的影響：

- 使用者無法刪除信箱中的專案。

- 受管理的資料夾助理無法刪除以保留標記或受管理的資料夾設定為基礎的專案。

- 針對已啟用單一專案復原或處於保留狀態的信箱，「寫入時複製」頁面保護程式無法維護使用者編輯的專案版本。

- 針對已啟用信箱審核記錄的信箱，[可復原的專案] 資料夾中的「審核」子資料夾中不能儲存任何信箱審核記錄專案。

對於未保留的信箱，系統管理員可以使用 `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell 中的命令來刪除 [可復原的專案] 資料夾中的專案。 如需詳細資訊，請參閱下列主題：

- [搜尋並刪除郵件](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

對於處於保留狀態的信箱，系統管理員必須先移除保留，然後才能從 [可復原的專案] 資料夾中刪除專案。 如需詳細資訊，請參閱 [刪除雲端式信箱的 [可復原的專案] 資料夾中的郵件暫止狀態](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。

為了協助防止 [可復原的專案] 資料夾成為已滿狀態，系統管理員可增加 [可復原的專案] 資料夾的儲存限制，以便保留信箱，並設定信箱保留原則，將專案從 [可復原的專案] 資料夾移至使用者的封存信箱。 請參閱 [增加保留信箱的可復原專案配額](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
