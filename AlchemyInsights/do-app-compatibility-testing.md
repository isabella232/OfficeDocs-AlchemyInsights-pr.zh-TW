---
title: 執行應用程式相容性測試
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529928"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="589c7-102">執行應用程式相容性測試</span><span class="sxs-lookup"><span data-stu-id="589c7-102">Do app compatibility testing</span></span>

<span data-ttu-id="589c7-103">Microsoft Edge 的應用程式相容性非常高。</span><span class="sxs-lookup"><span data-stu-id="589c7-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="589c7-104">事實上，它這麼高是因為 Microsoft 提供下列相容性承諾：</span><span class="sxs-lookup"><span data-stu-id="589c7-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="589c7-105">如果它可在 Microsoft Edge 45 和更舊版本上運作，則將可於 Microsoft Edge 77 及更新版本上運作。</span><span class="sxs-lookup"><span data-stu-id="589c7-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="589c7-106">如果它可以在 Internet Explorer 上運作，則將可以 Internet Explorer 模式在 Microsoft Edge 上運作。</span><span class="sxs-lookup"><span data-stu-id="589c7-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="589c7-107">如果它可以在 Google Chrome 上運作，則將可在 Microsoft Edge 上運作。</span><span class="sxs-lookup"><span data-stu-id="589c7-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="589c7-108">如果您有我們無法滿足此承諾的應用程式，我們會利用 [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure) 來修正以做為該承諾的後盾。</span><span class="sxs-lookup"><span data-stu-id="589c7-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="589c7-109">儘管有此承諾，我們知道許多組織基於合規性或風險管理理由，必須驗證某些應用程式。</span><span class="sxs-lookup"><span data-stu-id="589c7-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="589c7-110">雖然我們預期此作業會非常簡單，但對應用程式測試保持井然有序且嚴謹非常重要。</span><span class="sxs-lookup"><span data-stu-id="589c7-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="589c7-111">有兩種方式可以執行應用程式相容性測試：</span><span class="sxs-lookup"><span data-stu-id="589c7-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="589c7-112">**實驗室測試**：應用程式會在具有特定設定的嚴密控制環境中測試。</span><span class="sxs-lookup"><span data-stu-id="589c7-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="589c7-113">**試驗測試**：應用程式會由有限數量的使用者使用自己的裝置在每日工作環境中進行測試。</span><span class="sxs-lookup"><span data-stu-id="589c7-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="589c7-114">選擇最適合每個應用程式的方法，並在對整個組織啟動之前執行測試。</span><span class="sxs-lookup"><span data-stu-id="589c7-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="589c7-115">一旦確定您的應用程式相容，就可以準備將 Microsoft Edge 部署至試驗群組。</span><span class="sxs-lookup"><span data-stu-id="589c7-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
