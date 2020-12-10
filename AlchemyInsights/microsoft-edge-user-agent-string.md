---
title: 'Microsoft Edge 使用者代理程式字串 (桌面) '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2020
ms.locfileid: "49609569"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="b3abe-102">Microsoft Edge 使用者代理程式字串 (桌面) </span><span class="sxs-lookup"><span data-stu-id="b3abe-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="b3abe-103">使用者代理程式 (UA) 字串可用於偵測特定作業系統使用的特定瀏覽器版本。</span><span class="sxs-lookup"><span data-stu-id="b3abe-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="b3abe-104">就像其他瀏覽器，當使用者要求網站時，Microsoft Edge 會在「使用者代理程式」的 HTTP 標頭中包含這項資訊。</span><span class="sxs-lookup"><span data-stu-id="b3abe-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="b3abe-105">瀏覽器版本資訊也可以透過 JavaScript 來查詢「userAgent」的值。</span><span class="sxs-lookup"><span data-stu-id="b3abe-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="b3abe-106">我們建議 網頁程式開發人員盡可能使用功能偵測，以提升代碼可維護性、降低程式碼 fragility，以及消除未來 UA 字串更新時代碼破壞的風險。</span><span class="sxs-lookup"><span data-stu-id="b3abe-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="b3abe-107">如需詳細資訊，請參閱 [Microsoft Edge User Agent String (Desktop) ](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)。</span><span class="sxs-lookup"><span data-stu-id="b3abe-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>