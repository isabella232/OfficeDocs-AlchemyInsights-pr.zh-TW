---
title: 屬性和範圍篩選發生問題
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
- "8470"
- "9004687"
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960178"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>屬性和範圍篩選發生問題

**UPN 值衝突的問題**

Workday 至 AD 的使用者佈建顯示錯誤訊息 **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**。 作業失敗，因為針對新增/修改提供的 UPN 值並非全樹系唯一的值。 錯誤詳細資料：**CONSTRAINT_ATT_TYPE - userPrincipalName**。

目標 AD 網域已有建立 AD 使用者帳戶時 Workday 連接器嘗試設定的 **userPrincipalName** 值。 這表示 (1) 使用者已存在，且使用者的相符識別碼檢查失敗，或 (2) UPN 產生規則產生衝突值。

以下是建議解決方案的步驟：

如果使用者已存在且相符識別碼檢查無法將 Workday 帳戶連結至 Active Directory 帳戶，請檢查 Workday 和 AD 中的相符識別碼屬性 (通常是 **employeeID**)是否完全相符。 如果不相符，這是需要修正的資料問題。 例如，如果 Workday 中的 EmployeeID 是 001052，而 AD 中的是 1052，則佈建引擎將無法連結這兩個帳戶，且會嘗試建立已存在的使用者。 此案例中的解決方案是將 AD 中的 **EmployeeID** 值變更為包含前置數字零，即為 001052。
如果 UPN 產生的運算式未產生唯一值，請考慮使用重複資料刪除功能 **SelectUniqueValue**，以每次皆產生唯一值。

**Workday 至 AD 的使用者佈建未設定 AD 使用者帳戶的管理員屬性值**

Workday 至 AD 的使用者佈建工作未設定 AD 使用者帳戶的 **管理員** 屬性值。 出現此行為時，有兩種可能的情況：

1. 無法將 Workday 中的管理員解析為對應的 AD 使用者帳戶，因為該管理員不在範圍內。
2. 在 **多個 AD 網域** 情況中，Workday 中的管理員與使用者不在相同網域中。

請嘗試下列步驟以解決問題：

1. 如果您已定義範圍篩選，請先檢查管理員是否位於範圍內且滿足範圍子句。 如果管理員不符合範圍篩選準則，請變更篩選器，使管理員也位於佈建作業的範圍內。
2. 如果您有多個 AD 網域，則連接器具有已知的限制，即為無法解析跨網域管理員參照。

如需有關設定 Workday 以自動佈建的詳細資訊，請參閱[教學課程：設定 Workday 來自動佈建使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。













