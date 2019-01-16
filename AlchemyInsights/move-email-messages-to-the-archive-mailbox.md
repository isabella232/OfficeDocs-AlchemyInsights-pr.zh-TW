---
title: 將電子郵件移至封存信箱
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279378"
---
有問題封存的封存信箱的項目。請確定您已執行下列步驟：
  
1. 確認的**封存信箱**已啟用。如果不是，使用[本文](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes)中的步驟以啟用封存信箱。 
    
2. 在 Exchange 系統管理中心中，選取 [**相符性管理****保留標記**、 使用 [**移至封存**] 動作包含所需的**保留時間**建立**保留標記**。
    
3. 在 Exchange 系統管理中心中，選取 [**保留原則**、 建立**保留原則**並新增您**移至封存**保留標記至該原則。 
    
4. [將保留原則指派](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)給特定使用者的信箱。將相同的原則會套用至**主要**和**封存**信箱。 
    
使用者的信箱現在應該有將項目移至封存信箱的封存原則。可能需要強制受管理的資料夾助理員 (MFA) 執行並將新的設定套用至使用者的信箱。執行下列命令以啟動受管理的資料夾助理員特定信箱的同時[連線至 EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) ： 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

需要設定封存原則的詳細資訊，請參閱[Set up 信箱的封存及刪除原則](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。
  

