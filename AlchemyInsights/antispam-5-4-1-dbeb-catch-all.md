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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f3655-102">修正傳送問題的錯誤碼 550 5.4.1 轉送存取遭拒</span><span class="sxs-lookup"><span data-stu-id="f3655-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f3655-103">這個問題發生時[查看如果電子郵件地址時才有效防止 bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)輸入 Office 365 網路時。</span><span class="sxs-lookup"><span data-stu-id="f3655-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="f3655-104">請嘗試下列動作：</span><span class="sxs-lookup"><span data-stu-id="f3655-104">Try the following:</span></span>

1. <span data-ttu-id="f3655-105">判斷是否將整個網域或單一電子郵件地址的特定問題：</span><span class="sxs-lookup"><span data-stu-id="f3655-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f3655-106">整個網域： 有時網域需要進行同步處理;嘗試[設定內部網域，然後再回到授權](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)。</span><span class="sxs-lookup"><span data-stu-id="f3655-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f3655-107">單一電子郵件地址： 地址有時需要進行同步處理;變更的 smtp proxy 位址，然後變更回可以幫助。</span><span class="sxs-lookup"><span data-stu-id="f3655-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f3655-108">判斷問題是否為特定群組或公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="f3655-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f3655-109">對於某些物件類型，物件可能需要手動建立 Azure Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="f3655-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f3655-110">如果您需要其他協助，請開啟支援票證，並指定範圍的問題 (includidng 您要傳送至物件的類型)，我們可以協助您更好。</span><span class="sxs-lookup"><span data-stu-id="f3655-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>