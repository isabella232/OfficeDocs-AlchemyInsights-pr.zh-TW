---
title: Dynamics 365-Dynamics 365 整合介面中顯示錯誤的儀表板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528542"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="e39ca-102">Dynamics 365 整合介面中顯示錯誤的儀表板</span><span class="sxs-lookup"><span data-stu-id="e39ca-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="e39ca-103">有幾個理由為什麼您可能會看到比您預期不同儀表板：</span><span class="sxs-lookup"><span data-stu-id="e39ca-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="e39ca-104">使用者已設定的使用者預設儀表板</span><span class="sxs-lookup"><span data-stu-id="e39ca-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="e39ca-105">通常可以將使用者識別如果**設為預設值**] 按鈕不會顯示在儀表板命令列會設為預設儀表板。</span><span class="sxs-lookup"><span data-stu-id="e39ca-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="e39ca-106">使用者預設儀表板會覆寫所有其他預設儀表板，即使使用者的預設儀表板並不是在目前的應用程式中。</span><span class="sxs-lookup"><span data-stu-id="e39ca-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="e39ca-107">使用下列因應措施未設定其預設儀表板。</span><span class="sxs-lookup"><span data-stu-id="e39ca-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="e39ca-108">建立新的個人儀表板。</span><span class="sxs-lookup"><span data-stu-id="e39ca-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="e39ca-109">設定新儀表板的使用者預設值。</span><span class="sxs-lookup"><span data-stu-id="e39ca-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="e39ca-110">刪除儀表板。</span><span class="sxs-lookup"><span data-stu-id="e39ca-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="e39ca-111">在網站地圖中設定儀表板</span><span class="sxs-lookup"><span data-stu-id="e39ca-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="e39ca-112">您可以藉由選取儀表板，然後選擇 [設成預設值 '' 自訂系統 '] 下將設定組織預設儀表板。</span><span class="sxs-lookup"><span data-stu-id="e39ca-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="e39ca-113">但在網站地圖設計工具中定義的儀表板將優先於此儀表板，如果使用者具有其存取權。</span><span class="sxs-lookup"><span data-stu-id="e39ca-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="e39ca-114">若要讓使用者看到您已設定為組織預設儀表板，您可以：</span><span class="sxs-lookup"><span data-stu-id="e39ca-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="e39ca-115">在網站地圖中設定儀表板</span><span class="sxs-lookup"><span data-stu-id="e39ca-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="e39ca-116">移除這些使用者定義的網站地圖儀表板的存取</span><span class="sxs-lookup"><span data-stu-id="e39ca-116">Remove access to the sitemap defined dashboard for those users</span></span>
