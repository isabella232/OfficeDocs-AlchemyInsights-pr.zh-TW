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
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="f7049-102">修正錯誤代碼550的傳遞問題。5.4.1 轉送存取遭到拒絕</span><span class="sxs-lookup"><span data-stu-id="f7049-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="f7049-103">當您在進入 Microsoft 網路時， [檢查電子郵件地址是否有效以避免 bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) 時，就會發生此問題。</span><span class="sxs-lookup"><span data-stu-id="f7049-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="f7049-104">請嘗試下列動作：</span><span class="sxs-lookup"><span data-stu-id="f7049-104">Try the following:</span></span>

1. <span data-ttu-id="f7049-105">判斷問題是否因整個網域或單一電子郵件地址而異：</span><span class="sxs-lookup"><span data-stu-id="f7049-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="f7049-106">整個網域：有時候網域必須同步處理;嘗試 [將網域設定為 Internal，然後再將它設定為 [授權](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)]。</span><span class="sxs-lookup"><span data-stu-id="f7049-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="f7049-107">單一電子郵件地址：有時必須同步處理位址;變更 smtp proxy 位址，然後將其變更回來可協助您進行變更。</span><span class="sxs-lookup"><span data-stu-id="f7049-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="f7049-108">判斷問題是否因群組或公用資料夾而異。</span><span class="sxs-lookup"><span data-stu-id="f7049-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="f7049-109">在某些物件類型中，可能需要在 Azure Active Directory 中手動建立物件。</span><span class="sxs-lookup"><span data-stu-id="f7049-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="f7049-110">如果您需要其他協助，請開啟支援票證，並指定問題的範圍 (包含您要傳送至) 的物件類型，這樣我們就能協助您更好。</span><span class="sxs-lookup"><span data-stu-id="f7049-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>