---
title: Yammer 中的即時活動建立錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675433"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="f1069-102">Yammer 中的即時活動建立錯誤</span><span class="sxs-lookup"><span data-stu-id="f1069-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="f1069-103">**Yammer 即時活動建立**</span><span class="sxs-lookup"><span data-stu-id="f1069-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="f1069-104">Yammer 隨時會顯示用於建立即時活動的選項。</span><span class="sxs-lookup"><span data-stu-id="f1069-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="f1069-105">在某些情況下，使用者可能不符合建立即時事件的先決條件，並會在嘗試建立活動時收到錯誤。</span><span class="sxs-lookup"><span data-stu-id="f1069-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="f1069-106">下列項目涵蓋此問題的常見原因，並提供為終端使用者解決問題的方法。</span><span class="sxs-lookup"><span data-stu-id="f1069-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="f1069-107">**誰可以建立即時活動**</span><span class="sxs-lookup"><span data-stu-id="f1069-107">**Who can create live events**</span></span>
- <span data-ttu-id="f1069-108">Office 365 企業版 E1、E3 或 E5 授權，或 Office 365 A3 或 A5 授權。</span><span class="sxs-lookup"><span data-stu-id="f1069-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="f1069-109">對於在 Microsoft Teams 系統管理中心建立即時活動的權限。</span><span class="sxs-lookup"><span data-stu-id="f1069-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="f1069-110">對於在 Microsoft Stream 中建立即時活動的權限 (針對使用外部廣播應用程式或裝置產生的活動)。</span><span class="sxs-lookup"><span data-stu-id="f1069-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="f1069-111">組織中的完整小組成員資格 (不能是來賓或其他組織)。</span><span class="sxs-lookup"><span data-stu-id="f1069-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="f1069-112">私人會議排程、畫面共用及 IP 視訊共用，已在 Team 會議原則中開啟。</span><span class="sxs-lookup"><span data-stu-id="f1069-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="f1069-113">**即時活動建立原則**</span><span class="sxs-lookup"><span data-stu-id="f1069-113">**Live event creation policies**</span></span>

<span data-ttu-id="f1069-114">Yammer 遵循在您的 Office 365 租用戶中針對 Stream 設定的即時活動原則。</span><span class="sxs-lookup"><span data-stu-id="f1069-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="f1069-115">根據預設，貴組織中的所有人都可以建立即時活動。</span><span class="sxs-lookup"><span data-stu-id="f1069-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="f1069-116">系統管理員可[變更此設定，以防止使用者建立即時活動](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)。</span><span class="sxs-lookup"><span data-stu-id="f1069-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="f1069-117">如果使用者收到原則錯誤，請務必檢查使用者是否具有建立即時活動的權限。</span><span class="sxs-lookup"><span data-stu-id="f1069-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
