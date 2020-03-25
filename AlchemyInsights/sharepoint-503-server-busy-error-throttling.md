---
title: SharePoint 線上節流
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931217"
---
# <a name="sharepoint-online-throttling"></a>SharePoint 線上節流

**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。 包括內容遷移、資料遺失防護（DLP）及備份解決方案。 在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。

為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。 您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。 不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。

**503伺服器忙碌錯誤**

嘗試流覽至 SharePoint 或 OneDrive 網站時，使用者可能會收到503伺服器繁忙的錯誤。 

此錯誤可能是由 SharePoint 服務中的節流所造成。 SharePoint 線上使用節流，以維持 SharePoint 線上服務的最佳效能和可靠性。 節流限制使用者動作數目或並行通話（按腳本或程式碼）以避免過度使用資源。 

如需節流的詳細資訊，請參閱，[避免在線上 SharePoint 遭到節流或封鎖](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

如果您認為此錯誤與節流不相關，您可以流覽至[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)以檢查您租使用者上是否有使用中的維護。

 最後，請確定您已造訪 [[服務健康](https://portal.office.com/adminportal/home#/servicehealth)情況] 頁面，檢查任何可能發生的諮詢/事件。

