---
title: 使用者佈建
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430723"
---
# <a name="user-provisioning"></a>使用者佈建

- 使用 [隨選布建](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) 功能布建使用者，並取得所執行步驟的詳細診斷。
- 若要針對您在佈建使用者和群組時遇到的問題進行疑難排解，請參閱疑難排解指南[未佈建任何使用者](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)。
- 如果您發現未佈建使用者，請參閱在 Azure Active Directory (AD) 中[佈建記錄 (預覽)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)。 搜尋屬於特定使用者的記錄項目。
- 定期重新開機布建，以捕捉先前布建週期中錯過的任何使用者。
- 使用者/群組可能尚未布建，因為我們的服務尚未有機會評估使用者。 在 [布建設定] 頁面上，回顧布建所需的時間和進度列的指導方針。 如果 [其他詳細資料] 區段中所指定的穩定狀態是使用者建立/更新/刪除的日期，則表示尚未評估使用者。 在此案例中，最好的做法是等待布建服務完成。 如果已達到穩定狀態，我們建議您從 Azure 入口網站的 UI 執行重新開機。
  - 請注意，我們的服務只會注意到來源系統 (Azure Active Directory) 中的使用者/群組的變更。 如果使用者/群組是直接在應用程式中移除 (例如，ServiceNow) ，我們就不會注意到這些變更，而且不會根據來源系統中使用者的狀態將其退回。 在此案例中，最好直接復原目標應用程式中的變更。
- 我們的服務評估使用者/群組，並決定不應該布建：
  - 如果您已將範圍設定為 [指派的使用者和群組]，請檢查是否已將使用者/群組指派給應用程式。
  - 若使用者/群組已指派給應用程式，請確定其未指派給預設存取角色。 此角色不能用來進行布建。
  - 如果您已設定屬性架構範圍篩選，請確定使用者符合您指定的準則。
  - 如果使用者已存在於目標系統中，且來源和目標中的使用者狀態為 [符合]，我們將不會採取任何進一步的動作。
- 我們的服務嘗試布建使用者，但失敗。 在這些案例中，請參閱布建記錄檔的疑難排解與建議] 索引標籤：
  - 在 Azure Active Directory 中，使用者的必要屬性可能遺失或不符合協力廠商應用程式所需的格式。 例如，使用者的國家/地區屬性可能會設為美國。
  - 屬性是尚未存在於目標應用程式中的參照屬性。 參照屬性是指指向另一個物件的屬性，例如，屬於群組成員的使用者。 使用者的識別碼位於群組的 member 屬性中，但只有在它指向的使用者物件已存在時，才可以處理。
