---
title: 清單專案的批註
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724145"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="93516-102">清單專案的批註</span><span class="sxs-lookup"><span data-stu-id="93516-102">Comments on List items</span></span>

<span data-ttu-id="93516-103">使用者可以查看清單專案上的所有批註，並篩選顯示與專案相關的批註或活動的視圖。</span><span class="sxs-lookup"><span data-stu-id="93516-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="93516-104">使用者必須先注意下列專案，才能新增及刪除批註：</span><span class="sxs-lookup"><span data-stu-id="93516-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="93516-105">批註遵循 SharePoint 內做的許可權設定。</span><span class="sxs-lookup"><span data-stu-id="93516-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="93516-106">尚未建立以顯示在新式使用者介面（像是工作清單）中的傳統清單，將不會有這項批註功能。</span><span class="sxs-lookup"><span data-stu-id="93516-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="93516-107">在此版本中，不提供對小組中清單的批註。</span><span class="sxs-lookup"><span data-stu-id="93516-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="93516-108">不依搜尋編制索引的批註。</span><span class="sxs-lookup"><span data-stu-id="93516-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="93516-109">系統管理員可以在組織層級停用此功能，方法是在 **Set-SPOTenant** PowerShell Cmdlet 中變更 **CommentsOnListItemsDisabled** 參數。</span><span class="sxs-lookup"><span data-stu-id="93516-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="93516-110">目前不可能停用網站或清單層級的批註。</span><span class="sxs-lookup"><span data-stu-id="93516-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="93516-111">我們希望在後續的更新中使用這些控制項，這可能會在第一季度2021。</span><span class="sxs-lookup"><span data-stu-id="93516-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
