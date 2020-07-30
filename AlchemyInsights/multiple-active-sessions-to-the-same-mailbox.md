---
title: 同一郵箱的多个作用中的工作階段
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431407"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="7f25b-102">同一郵箱的多个作用中的工作階段</span><span class="sxs-lookup"><span data-stu-id="7f25b-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="7f25b-103">若要控制 Exchange 資源的使用情況，信箱中有「預算」。</span><span class="sxs-lookup"><span data-stu-id="7f25b-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="7f25b-104">超出預算的例外狀況可被觸發，但不限於下列情況：</span><span class="sxs-lookup"><span data-stu-id="7f25b-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="7f25b-105">在同一 Outlook Web App 工作階段中開啟了幾個瀏覽器索引標籤。</span><span class="sxs-lookup"><span data-stu-id="7f25b-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="7f25b-106">同一信箱的幾個使用中的 Outlook Web App 的工作階段。</span><span class="sxs-lookup"><span data-stu-id="7f25b-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="7f25b-107">其他一些用戶端應用程式 (Outlook、Outlook Mobile、協力廠商用戶端應用程式) 可同時存取信箱。</span><span class="sxs-lookup"><span data-stu-id="7f25b-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="7f25b-108">長期執行的作業 (例如執行搜尋請求) 會在另一個使用中的信箱工作階段執行。</span><span class="sxs-lookup"><span data-stu-id="7f25b-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

