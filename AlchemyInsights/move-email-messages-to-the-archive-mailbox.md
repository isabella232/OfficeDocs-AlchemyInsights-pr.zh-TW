---
title: 將電子郵件移至封存信箱
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418283"
---
# <a name="move-email-to-the-archive-mailbox"></a>將電子郵件移至封存信箱
 
1. 確認的**封存信箱**已啟用。 否則，請使用[本文](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)中的步驟，以啟用封存信箱。

2. 若要封存自動至封存信箱的郵件，具有 [**移至封存**] 動作的保留標記必須設**至整個信箱 （預設值） 標籤自動套用**。 在這裡使用的步驟，來建立標記：[預設封存標記](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)。
    
3. 接下來，將**封存**標記新增至保留原則。 在 Exchange 系統管理中心中，選擇 [**保留原則**> 來**儲存**原則 > 新增 [**移至封存] 標記**。 
    
4. 接下來[將保留原則指派](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)給特定使用者的信箱。 相同的原則會套用至**主要**和**封存**信箱。 
    
它可能需要強制執行受管理的資料夾助理員 (MFA) 執行，並將新的設定套用至使用者的信箱。 執行下列命令以啟動受管理的資料夾助理員特定信箱的同時[連接至 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) : 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

如需有關封存原則設定的詳細資訊，請參閱 < <b0>Set up 信箱的封存和刪除原則</b0>。
  

