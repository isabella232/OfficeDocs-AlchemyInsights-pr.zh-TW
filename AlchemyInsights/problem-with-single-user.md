---
title: 單一使用者的問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428691"
---
# <a name="problem-with-single-user"></a>單一使用者的問題

- 使用者可能尚未布建，因為服務尚未有機會評估使用者。 在 [布建設定] 頁面上，回顧布建所需的時間和進度列的指導方針。 如果 [其他詳細資料] 區段中所指定的穩定狀態是使用者建立/更新/刪除的日期，則表示尚未評估使用者。 在此案例中，最好的做法是等待布建服務完成。

  - 請注意，我們的服務只會注意到來源系統中的使用者變更 (Cloud HR) 。 Azure AD 的來源系統中必須有有效的變更，才能偵測變更，並將其流式傳送至 Active Directory。
- 布建服務評估使用者並決定不應該布建：
  - 如果您已設定屬性架構範圍篩選，請確定使用者符合您指定的準則。
  - 如果使用者已存在於目標系統中，且來源和目標中的使用者狀態為 [符合]，我們將不會採取任何進一步的動作。
- 布建服務嘗試布建使用者，但失敗。 在這些案例中，請參閱布建記錄檔的疑難排解與建議] 索引標籤：
  - 在內部部署 Active Directory 或 Azure AD 中，使用者的必要屬性可能遺失。 例如，userPrincipalName 或 sAMAccountName 產生規則不會產生正確的值。
  - 在內部部署 Active Directory 或 Azure AD 中，[) 公司單位] 的相符屬性 (通常不會解析為唯一的使用者。 例如，在 AD 中有兩位使用者有相同的雇員 Id，且該服務傳回錯誤碼，表示相同來源專案的重複目標專案。

若要查看單一使用者和群組的記錄，請參閱針對 [特定使用者的問題複查](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)布建記錄檔。
