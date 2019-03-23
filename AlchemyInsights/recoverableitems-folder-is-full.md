---
title: 1336 RecoverableItems 資料夾已滿
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: a048949d5284d018303d03aad26cdf26eee2fb5c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776388"
---
# <a name="the-recoverable-items-folder-is-full"></a>[可復原的項目] 資料夾已滿

在 Office 365 中的 Exchange Online 信箱，[可復原的項目] 資料夾的預設儲存量限制為 30 GB。 如果信箱處於訴訟暫止狀態，eDiscovery 保留] 中，或指派給 Office 365 保留原則，[可復原的項目] 資料夾的儲存量限制會自動增加到 100GB。
  
當 [可復原的項目] 資料夾達到儲存量限制時，是以下列方式影響信箱功能：
  
- 使用者無法從信箱中刪除項目。
    
- 受管理的資料夾助理員無法刪除保留標記或受管理的資料夾設定為基礎的項目。
    
- 啟用單一項目復原或會處於保留狀態的信箱，寫入時複製頁面保護程序無法維護版本的使用者編輯項目。
    
- 針對已啟用信箱稽核記錄的信箱，沒有信箱稽核記錄項目可以儲存在 [可復原的項目] 資料夾中的 [稽核] 子資料夾中。
    
針對不保留的信箱，系統管理員可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent`命令在 Exchange Online PowerShell 中刪除 [可復原的項目] 資料夾中的項目。 如需相關資訊，請參閱下列主題： 
  
- [搜尋並刪除郵件](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [搜尋信箱](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
針對要保留的信箱，系統管理員必須移除保留，他們可以從 [可復原的項目] 資料夾刪除項目之前。 如需詳細資訊，請參閱 <<c0>可復原的項目保留的雲端架構信箱上的資料夾內刪除項目。
  
若要協助防止成為完整 [可復原的項目] 資料夾，系統管理員可以增加可復原的項目資料夾信箱的保留和設定將項目從 [可復原的項目] 資料夾移至使用者的封存的信箱保留原則的儲存限制信箱。 請參閱[增加可復原的項目配額的信箱保留](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
  

