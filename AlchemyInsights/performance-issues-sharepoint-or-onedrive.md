---
title: 效能問題-SharePoint 或 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771892"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint 或 OneDrive 多個使用者的慢速、無法存取或無法使用

SharePoint 或 OneDrive 可能會變慢、無法存取或無法使用，或顯示服務無法使用或503錯誤，其原因有多種：
  
- 如果您的 SharePoint 或 OneDrive 網站的執行速度很慢或延遲多個使用者，則在存取 SharePoint 網站或 OneDrive 內容時，使用者可能會遇到延遲延遲或流覽錯誤的暫時性服務問題。 請查看[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解您的組織是否受到影響。
  
- 嘗試流覽至 SharePoint 或 OneDrive 網站時，使用者可能會收到 *503 伺服器繁忙* 的錯誤。 此錯誤可能是由 SharePoint 服務中的節流所造成。 SharePoint Online 會使用節流來維護 SharePoint Online 服務的最佳效能和可靠性。 節流會限制使用者動作或同時通話的數目 (藉由指令碼或程式碼)，以避免過度使用資源。 如需節流的詳細資訊，請參閱， [避免在線上 SharePoint 遭到節流或封鎖](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

- 如果您使用 **傳統** 或 **新式** SharePoint 網站或頁面時速度變慢，請利用 [頁面診斷工具](https://aka.ms/perftool) 來分析頁面。
  
- 如果您仍遇到一般緩慢效能，請參閱本文底部的資源： [SharePoint 線上的效能調整簡介](https://go.microsoft.com/fwlink/?linkid=2024334)
  