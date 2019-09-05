---
title: 疑難排解問題-目錄中找不到使用者
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754183"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>疑難排解問題-目錄中找不到使用者

如果使用者會收到錯誤訊息 「 使用者找不到 」 目錄中。 請再試一次其中問題類型是使用者不在目錄中。

若要疑難排解問題，可以完成下列步驟。

- 確定公認的電子郵件邀請是相同的帳戶是用來以稍後再登入的帳戶。 請確定使用者以接受邀請，並登入網站使用相同的帳戶。 

如需詳細資訊，請參閱[如何管理您的 Microsoft 帳戶的別名</a>來管理 Office 365 登入](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)。 

- 瀏覽至每個網站中的使用者會收到錯誤。 

新增 「 / _layouts/15/people.aspx/membershipgroupid=0 」 （內雙引號） 的網站 URL 的結尾。 

範例： https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。

- 從清單中選取使用者。

- 按一下 [從功能區的 [**移除使用者權限**。 
-  將使用者新增回並重新邀請傳送給使用者。

