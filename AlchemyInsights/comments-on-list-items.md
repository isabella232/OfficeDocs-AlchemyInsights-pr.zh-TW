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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947488"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="1c51b-102">清單專案的批註</span><span class="sxs-lookup"><span data-stu-id="1c51b-102">Comments on List items</span></span>

<span data-ttu-id="1c51b-103">使用者將很快可以新增及刪除清單專案的批註。</span><span class="sxs-lookup"><span data-stu-id="1c51b-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="1c51b-104">使用者可以查看清單專案上的所有批註，並篩選顯示與專案相關的批註或活動的視圖。</span><span class="sxs-lookup"><span data-stu-id="1c51b-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="1c51b-105">**計時** ：</span><span class="sxs-lookup"><span data-stu-id="1c51b-105">**Timing** :</span></span>

<span data-ttu-id="1c51b-106">**目標版本** ：逐步推出于十月，預計會在2006年11月完成</span><span class="sxs-lookup"><span data-stu-id="1c51b-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="1c51b-107">**標準版本** ：逐步推出，在十二月的初期完成</span><span class="sxs-lookup"><span data-stu-id="1c51b-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="1c51b-108">**首展** ：整個組織的目標發行</span><span class="sxs-lookup"><span data-stu-id="1c51b-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="1c51b-109">使用者必須先注意下列專案，才能新增及刪除批註：</span><span class="sxs-lookup"><span data-stu-id="1c51b-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="1c51b-110">批註遵循 SharePoint 內做的許可權設定。</span><span class="sxs-lookup"><span data-stu-id="1c51b-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="1c51b-111">尚未建立以顯示在新式使用者介面（像是工作清單）中的傳統清單，將不會有這項批註功能。</span><span class="sxs-lookup"><span data-stu-id="1c51b-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="1c51b-112">在此版本中，不提供對小組中清單的批註。</span><span class="sxs-lookup"><span data-stu-id="1c51b-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="1c51b-113">不依搜尋編制索引的批註。</span><span class="sxs-lookup"><span data-stu-id="1c51b-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="1c51b-114">系統管理員可以在組織層級停用此功能，方法是在 **Set-SPOTenant** PowerShell Cmdlet 中變更 **CommentsOnListItemsDisabled** 參數。</span><span class="sxs-lookup"><span data-stu-id="1c51b-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="1c51b-115">目前不可能停用網站或清單層級的批註。</span><span class="sxs-lookup"><span data-stu-id="1c51b-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="1c51b-116">我們希望在後續的更新中使用這些控制項，這可能會在第一季度2021。</span><span class="sxs-lookup"><span data-stu-id="1c51b-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
