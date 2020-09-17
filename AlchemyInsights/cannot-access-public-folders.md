---
title: 無法存取公用資料夾
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812538"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 無法連接至公用資料夾

如果公用資料夾存取無法為某些使用者運作，請嘗試下列步驟：

連線至 EXO PowerShell，並在有問題的使用者帳戶上設定 DefaultPublicFolderMailbox 參數，以與使用中使用者帳戶的參數相符。

範例：

Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

至少等候一個小時，讓變更生效。

如果問題仍然存在， [請執行下列程式，以](https://aka.ms/pfcte) 使用 Outlook 疑難排解公用資料夾存取問題。
 
**若要控制哪些使用者可以使用 Outlook 存取公用資料夾**：

1.  使用 Set-CASMailbox <mailboxname> PublicFolderClientAccess $true 或 $false  
      
    $true：允許使用者在 Outlook 中存取公用資料夾  
      
    $false：避免使用者在 Outlook 中存取公用資料夾。 這是預設值。  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**記事** 此程式只能控制 Outlook desktop for Windows 用戶端的連線。 使用者可以繼續使用 OWA 或 Outlook for Mac 來存取公用資料夾。
 
如需詳細資訊，請參閱 [宣佈對 Outlook 中公用資料夾的可控連線支援](https://aka.ms/controlpf)。