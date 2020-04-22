---
title: 疑難排解問題-在目錄中找不到使用者
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702729"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>疑難排解問題-在目錄中找不到使用者

如果使用者在目錄中收到錯誤訊息「找不到使用者」，請再試一次問題類型為使用者不在目錄中的地方。

您可以完成下列步驟以進行問題的疑難排解。

- 確定接受的電子郵件邀請的帳戶與以後用於登入的帳戶相同。 請確定使用者使用相同的帳戶來接受邀請並登入網站。 

如需詳細資訊，請參閱 how [to 365 manage</a> ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)a a a a a a a a a a a a a a 

- 流覽至使用者收到錯誤的每個網站。 

在網站 URL 的結尾新增 "/_layouts/15/people.aspx/membershipgroupid = 0" （雙引號內）。 

範例： HTTPs://< "contoso" > sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。

- 從清單中選取使用者。

- 按一下功能區中的 [**移除使用者**權力]。 
-  新增回使用者，然後將邀請重新傳送給使用者。

