---
title: MC210173 - SharePoint Designer 新自訂表單功能取代
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928519"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="44d9c-102">MC210173 - SharePoint Designer 新自訂表單功能取代</span><span class="sxs-lookup"><span data-stu-id="44d9c-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="44d9c-103">我們已找出會影響 SharePoint Designer 功能在 SharePoint Online 中[建立自訂表單](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)的問題。</span><span class="sxs-lookup"><span data-stu-id="44d9c-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="44d9c-104">仔細檢查之後，我們判定此問題的沒有已知修正程式，並已選擇停用自訂表單建立功能 (自 2020 年 4 月 25 日星期六上午 3:00 UTC 起生效)。</span><span class="sxs-lookup"><span data-stu-id="44d9c-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="44d9c-105">這項變更不會影響在 SharePoint Online Designer 中編輯先前建立的表單或其他現有功能的能力。</span><span class="sxs-lookup"><span data-stu-id="44d9c-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="44d9c-106">進行此變更之後，使用者可能已收到以下錯誤：「建立新表單時，無法將清單變更儲存到伺服器」。</span><span class="sxs-lookup"><span data-stu-id="44d9c-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="44d9c-107">先前使用 SharePoint Designer 建立自訂表單的使用者，可以將 [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) 用於此目的。</span><span class="sxs-lookup"><span data-stu-id="44d9c-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="44d9c-108">PowerApps 是一種簡易且功能強大的工具，可讓在 SharePoint Online 新式體驗中操作的使用者，直接從瀏覽器視窗建立及編輯 SharePoint 清單和文件庫的自訂表單。</span><span class="sxs-lookup"><span data-stu-id="44d9c-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="44d9c-109">PowerApps 不需要傳統編碼知識，或下載任何其他應用程式，例如 InfoPath。</span><span class="sxs-lookup"><span data-stu-id="44d9c-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="44d9c-110">**注意**：SharePoint Online 傳統版使用者將需要暫時切換到新式體驗，才能存取和使用 PowerApps；不過，在 PowerApps 中建立的所有自訂表單均可由 SharePoint Online 傳統版體驗使用者存取。</span><span class="sxs-lookup"><span data-stu-id="44d9c-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
