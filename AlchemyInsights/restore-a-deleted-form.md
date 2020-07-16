---
title: 還原已刪除的表單
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 246c3b50df856c16ea5237adc43d2126bb5b48b9
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148028"
---
# <a name="restore-a-deleted-form"></a>還原已刪除的表單

如果您已意外刪除 Microsoft Forms 中的表單，可以進行復原。 以刪除之表單的擁有者身分登入 Microsoft Forms。 選取 [**回收站**]，然後選取您要復原的表單，然後選取 [**還原**]。 還原後，選取 [**回到我的表單] 頁面**箭號。

只有表單的擁有者可以復原。 如果已停用或移除租使用者的帳戶，則只有全域系統管理員才能復原表單。 全域管理員必須具備表單會授權，才可執行還原。 只有在停用的使用者帳戶的30天內建立或從承租人中移除的表單，才能還原。

如果您是租使用者的全域系統管理員，而您想要從已刪除或已停用的帳戶復原表單，請將 [電子郵件地址] 取代為下列 URL: ** https://forms.office.com/Pages/delegatepage.aspx?originalowner= [電子郵件地址]** 中已刪除或已停用之使用者的電子郵件地址。例如，如果您的電子郵件地址是 JOHNDOE@CONTOSO.COM，則 URL 會是： **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** 。 

一旦您可以存取使用者的已刪除表單，請選取您要移動的表單，然後選取 [**其他表單動作**  >  **移動**]。

若要復原已刪除但已從組織中移除使用者的表單，全域管理員可以選擇復原使用者、重設使用者的密碼，然後在以該使用者的身分登入時，存取表單，將其移至另一個作用中的使用者。 