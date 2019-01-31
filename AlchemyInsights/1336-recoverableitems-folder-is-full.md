---
title: 1336 RecoverableItems 資料夾已滿
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: b8b3e5389778b3aff0fbe2f6506ba2b2fc3abc7e
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655658"
---
# <a name="the-recoverable-items-folder-is-full"></a>可復原的項目] 資料夾已滿

Office 365 中的 Exchange Online 信箱，可復原的項目] 資料夾的預設儲存量限制為 30 GB。如果信箱處於訴訟暫止狀態、 eDiscovery 保留或指派給 Office 365 保留原則可復原的項目] 資料夾的儲存量限制自動增加為 100 GB。
  
可復原的項目] 資料夾達到的儲存量限制，信箱功能受到方式如下：
  
- 使用者無法從信箱刪除項目。
    
- 受管理的資料夾助理員無法刪除保留標記或受管理的資料夾設定為基礎的項目。
    
- 信箱已啟用單一項目復原或保留寫入時複製頁面保護程序無法維護版本的使用者所編輯的項目。
    
- 擁有信箱稽核記錄已啟用的信箱，沒有信箱稽核記錄項目可以儲存在 [可復原的項目] 資料夾中的稽核子資料夾中。
    
不保留的信箱，系統管理員可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent`命令在 Exchange Online PowerShell 內可復原的項目] 資料夾刪除項目。如需詳細資訊，請參閱下列主題： 
  
- [搜尋並刪除郵件](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
保留上的信箱，系統管理員必須移除保留他們可以從 [可復原的項目] 資料夾刪除的項目之前。如需詳細資訊，請參閱[可復原的項目保留的雲端架構信箱上的資料夾內刪除項目](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。
  
為了協助防止變成完整可復原的項目] 資料夾，系統管理員可以提高儲存限制的可復原的項目資料夾上信箱保留並將項目從 [可復原的項目] 資料夾移至使用者的封存信箱保留原則設定信箱。請參閱[增加保留上的信箱配額可復原的項目](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。
  

