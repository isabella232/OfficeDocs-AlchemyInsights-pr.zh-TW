---
title: 執行應用程式相容性測試
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529928"
---
# <a name="do-app-compatibility-testing"></a>執行應用程式相容性測試

Microsoft Edge 的應用程式相容性非常高。 事實上，它這麼高是因為 Microsoft 提供下列相容性承諾：
- 如果它可在 Microsoft Edge 45 和更舊版本上運作，則將可於 Microsoft Edge 77 及更新版本上運作。
- 如果它可以在 Internet Explorer 上運作，則將可以 Internet Explorer 模式在 Microsoft Edge 上運作。
- 如果它可以在 Google Chrome 上運作，則將可在 Microsoft Edge 上運作。

如果您有我們無法滿足此承諾的應用程式，我們會利用 [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure) 來修正以做為該承諾的後盾。

儘管有此承諾，我們知道許多組織基於合規性或風險管理理由，必須驗證某些應用程式。 雖然我們預期此作業會非常簡單，但對應用程式測試保持井然有序且嚴謹非常重要。

有兩種方式可以執行應用程式相容性測試：

- **實驗室測試**：應用程式會在具有特定設定的嚴密控制環境中測試。
- **試驗測試**：應用程式會由有限數量的使用者使用自己的裝置在每日工作環境中進行測試。

選擇最適合每個應用程式的方法，並在對整個組織啟動之前執行測試。

一旦確定您的應用程式相容，就可以準備將 Microsoft Edge 部署至試驗群組。
