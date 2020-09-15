---
title: Dynamics 365-Dynamics 365 統一介面中顯示錯誤的儀表板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711266"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="aa1ea-102">Dynamics 365 統一介面中顯示錯誤的儀表板</span><span class="sxs-lookup"><span data-stu-id="aa1ea-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="aa1ea-103">您看到的儀表板可能與您預期的不同，原因如下：</span><span class="sxs-lookup"><span data-stu-id="aa1ea-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="aa1ea-104">使用者已設定使用者預設儀表板</span><span class="sxs-lookup"><span data-stu-id="aa1ea-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="aa1ea-105">一般來說，如果 [ **設定為預設** 值] 按鈕未顯示在儀表板命令列中，您可以識別使用者預設的儀表板。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="aa1ea-106">使用者預設儀表板會覆寫所有其他的預設儀表板，即使使用者的預設儀表板不在目前的應用程式中也是一樣。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="aa1ea-107">請使用下列解決方法來取消設置其預設儀表板。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="aa1ea-108">建立新的個人儀表板。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="aa1ea-109">將新的儀表板設定為使用者預設。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="aa1ea-110">刪除該儀表板。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="aa1ea-111">儀表板是在網站地圖中設定</span><span class="sxs-lookup"><span data-stu-id="aa1ea-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="aa1ea-112">您可以選取儀表板，然後選擇 [自訂系統] 底下的 [設為預設值]，以設定組織的預設儀表板。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="aa1ea-113">不過，如果使用者可以存取，則在網站地圖設計工具中定義的儀表板會優先于此儀表板。</span><span class="sxs-lookup"><span data-stu-id="aa1ea-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="aa1ea-114">若要讓使用者看到您已設定為組織預設的儀表板，您可以執行下列其中一項操作：</span><span class="sxs-lookup"><span data-stu-id="aa1ea-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="aa1ea-115">在網站地圖中設定該儀表板</span><span class="sxs-lookup"><span data-stu-id="aa1ea-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="aa1ea-116">移除對那些使用者的網站地圖定義儀表板的存取權</span><span class="sxs-lookup"><span data-stu-id="aa1ea-116">Remove access to the sitemap defined dashboard for those users</span></span>
