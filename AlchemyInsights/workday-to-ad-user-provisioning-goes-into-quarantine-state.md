---
title: Workday 至 AD 使用者佈建進入隔離狀態
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036483"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday 至 AD 使用者佈建進入隔離狀態

**Workday 至 AD 使用者佈建進入隔離狀態且 AD 中未建立使用者**

Workday 至 AD 使用者佈建工作進入隔離狀態，稽核記錄顯示匯出失敗事件，出現錯誤訊息 **錯誤：OperationsError-SvcErr：發生作業錯誤。尚未為目錄服務設定上層參照。目錄服務因此無法發行轉介給這個樹系外的物件**。 此錯誤通常在 Active Directory 容器 OU 未正確設定，或用於 **parentDistinguishedName** 的運算式對應發生問題時顯示。

檢查 **新使用者** 參數的預設 OU 是否輸入錯誤。 確保指定的 OU 已存在於您的 AD 中。 如果您在屬性對應中使用 **parentDistinguishedName**，請確保其一律評估為 AD 網域中的已知容器。 檢查稽核記錄中的匯出事件，以查看產生的值。

如需有關設定 Workday 以自動佈建的詳細資訊，請參閱[教學課程：設定 Workday 來自動佈建使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。

