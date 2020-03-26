---
title: SharePoint 移轉效能
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931882"
---
# <a name="sharepoint-migration-performance"></a>SharePoint 移轉效能

**重要**：許多 SharePoint Online 和 OneDrive 客戶都會對在背景中執行的服務執行關鍵應用程式。 其中包括內容移轉、資料遺失防護 (DLP) 及備份解決方案。 在這些前所未有的情況中，我們會採取一些步驟來確保 SharePoint Online 和 OneDrive 服務保持高度可用和可靠的狀態，以便在遠端工作情況下比以往更依賴服務的使用者使用。

為了支持這個目標，我們已在平日白天時段內對背景應用程式 (移轉、DLP 和備份解決方案) 上實施更嚴密的節流限制。 在這些情況中，您會認為這些應用程式的輸送量相當有限。 不過，在夜間和週末時段內，服務將會準備好處理來自背景應用程式的更大量要求。

**移轉效能**

移轉效能可能會受到網路基礎結構、檔案大小、移轉時間和節流的影響。了解這些可協助您規劃並最佳化您的移轉效能。

如需詳細資訊，請瀏覽以下連結。

- [SharePoint Online 和 ODB 的移轉速度](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [如何避免在 SharePoint Online 中受到節流控制或封鎖](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [下載並安裝 SharePoint 移轉工具](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
