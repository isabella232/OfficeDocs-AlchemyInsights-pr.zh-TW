---
title: Microsoft Edge 設定隱私權設定
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114163"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge 設定隱私權設定

根據預設，如果 Microsoft Edge 部署在非 Windows 的平臺上，診斷資料和網站資訊不會傳送給 Microsoft。 不過，如果 Microsoft Edge 部署在 Windows 10 上，則會根據使用者的[Windows 診斷資料設定](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)來傳送診斷資料和網站資訊。

若要設定 Microsoft Edge 如何處理組織的資料收集，請使用下列群組原則：
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)：這個原則可讓您報告使用狀況及與損毀相關的資料。
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)：此原則會傳送用來改善 Microsoft 服務的網站資訊。

若要深入瞭解，請參閱 [設定原則設定](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)。