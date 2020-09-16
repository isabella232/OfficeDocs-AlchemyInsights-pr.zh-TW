---
title: MC210173 - SharePoint Designer 新自訂表單功能取代
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
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: a53b8885a877cb688cfb42bb4f9108cb2cef2418
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743744"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePoint Designer 新自訂表單功能取代

我們已找出會影響 SharePoint Designer 功能在 SharePoint Online 中[建立自訂表單](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)的問題。 仔細檢查之後，我們判定此問題的沒有已知修正程式，並已選擇停用自訂表單建立功能 (自 2020 年 4 月 25 日星期六上午 3:00 UTC 起生效)。 這項變更不會影響在 SharePoint Online Designer 中編輯先前建立的表單或其他現有功能的能力。

進行此變更之後，使用者可能已收到以下錯誤：「建立新表單時，無法將清單變更儲存到伺服器」。

先前使用 SharePoint Designer 建立自訂表單的使用者，可以將 [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) 用於此目的。

PowerApps 是一種簡易且功能強大的工具，可讓在 SharePoint Online 新式體驗中操作的使用者，直接從瀏覽器視窗建立及編輯 SharePoint 清單和文件庫的自訂表單。 PowerApps 不需要傳統編碼知識，或下載任何其他應用程式，例如 InfoPath。

**注意**：SharePoint Online 傳統版使用者將需要暫時切換到新式體驗，才能存取和使用 PowerApps；不過，在 PowerApps 中建立的所有自訂表單均可由 SharePoint Online 傳統版體驗使用者存取。
