---
title: 在 Microsoft Edge 中設定隱私權設定
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403814"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>在 Microsoft Edge 中設定隱私權設定

根據預設，如果 Microsoft Edge 部署在非 Windows 平臺上，則診斷資料和網站資訊不會傳送給 Microsoft。 不過，如果 Microsoft Edge 部署在 Windows 10 上，診斷資料和網站資訊會根據使用者的 [Windows 診斷資料設定](https://go.microsoft.com/fwlink/?linkid=2132472)傳送。

若要設定 Microsoft Edge 如何處理組織的資料收集，請使用下列群組原則：
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) 開啟使用狀況和崩潰相關資料的報告。
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) 會傳送用來改善 Microsoft 服務的網站資訊。

若要深入瞭解，請參閱 [設定原則設定](https://go.microsoft.com/fwlink/?linkid=2132577)。
