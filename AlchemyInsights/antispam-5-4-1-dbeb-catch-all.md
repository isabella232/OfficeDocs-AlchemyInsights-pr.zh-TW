---
title: 反垃圾郵件 5.4.1 DBEB 全部
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672424"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>修正傳送問題的錯誤碼 550 5.4.1 轉送存取遭拒

這個問題發生時[查看如果電子郵件地址時才有效防止 bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)輸入 Office 365 網路時。 請嘗試下列動作：

1. 判斷是否將整個網域或單一電子郵件地址的特定問題：
    - 整個網域： 有時網域需要進行同步處理;嘗試[設定內部網域，然後再回到授權](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)。
    - 單一電子郵件地址： 地址有時需要進行同步處理;變更的 smtp proxy 位址，然後變更回可以幫助。
2. 判斷問題是否為特定群組或公用資料夾。 對於某些物件類型，物件可能需要手動建立 Azure Active Directory 中。

如果您需要其他協助，請開啟支援票證，並指定範圍的問題 (includidng 您要傳送至物件的類型)，我們可以協助您更好。