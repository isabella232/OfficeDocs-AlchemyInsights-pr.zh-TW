---
title: 反垃圾郵件 5.4.1 DBEB 全部捕獲
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717352"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>修正錯誤代碼550的傳遞問題。5.4.1 轉送存取遭到拒絕

當您在進入 Microsoft 網路時， [檢查電子郵件地址是否有效以避免 bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) 時，就會發生此問題。 請嘗試下列動作：

1. 判斷問題是否因整個網域或單一電子郵件地址而異：
    - 整個網域：有時候網域必須同步處理;嘗試 [將網域設定為 Internal，然後再將它設定為 [授權](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)]。
    - 單一電子郵件地址：有時必須同步處理位址;變更 smtp proxy 位址，然後將其變更回來可協助您進行變更。
2. 判斷問題是否因群組或公用資料夾而異。 在某些物件類型中，可能需要在 Azure Active Directory 中手動建立物件。

如果您需要其他協助，請開啟支援票證，並指定問題的範圍 (包含您要傳送至) 的物件類型，這樣我們就能協助您更好。