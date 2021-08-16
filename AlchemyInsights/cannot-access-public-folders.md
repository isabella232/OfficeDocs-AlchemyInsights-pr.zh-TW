---
title: 無法存取公用資料夾
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996621"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 無法連接至公用資料夾

如果公用資料夾存取無法為某些使用者運作，請嘗試下列步驟：

連線以 EXO PowerShell 並設定問題使用者帳戶上的 DefaultPublicFolderMailbox 參數，使其符合工作的使用者帳戶上的參數。

例如:

Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

至少等候一個小時，讓變更生效。

如果問題仍然存在，[請依照下列](https://aka.ms/pfcte)程式使用 Outlook 來疑難排解公用資料夾存取問題。
 
**若要控制哪些使用者可以使用 Outlook 存取公用資料夾**：

1.  使用 Set-CASMailbox <mailboxname> PublicFolderClientAccess $true 或 $false  
      
    $true：允許使用者在 Outlook 中存取公用資料夾  
      
    $false：避免使用者在 Outlook 中存取公用資料夾。 這是預設值。  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**記事** 此程式僅能控制 Windows 用戶端的 Outlook 桌面連接。 使用者可以使用 OWA 或 Mac 版 Outlook 繼續存取公用資料夾。
 
如需詳細資訊，請參閱[在 Outlook 中，宣佈對公用資料夾的受控連線支援](https://aka.ms/controlpf)。