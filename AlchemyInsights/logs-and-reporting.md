---
title: 記錄與報告
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067003"
---
# <a name="logs-and-reporting"></a>記錄與報告

[Azure Active Directory 報告常見問題](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq)回答 Azure Active Directory (Azure AD) 報告相關的常見問題。 如需詳細資訊，請參閱[Azure Active Directory 報告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)。

**對審計問題進行疑難排解**

1. 如果您在查看某些審核活動時發生問題，但在此 [清單](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)中找不到活動，請將支援票證檔。
2. 如果您在租使用者中查看任何審計記錄檔時遇到問題，請提供支援憑證。
3. 如果您的審計活動不會立即顯示在 Azure 入口網站中，請查看延遲 [資訊](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) 和檔案 a 支援票證（如果延遲超過所記錄的延遲）。
4. [Azure AD 活動記錄保留](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. 如果您沒有看到您所選取之日期範圍的所有審計，您可以下載最多250K 列 (從 Azure 入口網站的最近) 登入排序。 如需詳細資訊，請參閱 [審核活動下載](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)。

**疑難排解登錄問題**

1. 如果您擁有租使用者 (P1 或 P2) 授權的 Azure AD Premium，您只會看到過去的30天的資料。
2. 只有 Azure AD Premium 承租人才能使用登入。 無法使用免費或基本授權承租人。
3. 如果您的租使用者有進階版 P1 授權，但您看不到登入，請查看我們的[延遲資訊](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)，並在延遲超過所記錄的延遲時，將支援憑證。
4. 如果您沒有看到您所選取之日期範圍的所有登入，請注意，您最多可以下載250K 列 (從 Azure 入口網站的最近) 登入排序。 如需詳細資訊，請參閱登 [入活動下載](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)。

**疑難排解安全報告 (已標記為危險的使用者 Sign-In)**

1. [已標記風險安全性報告的使用者](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [Azure Active Directory 入口網站中的危險登入報告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [Azure Active Directory 風險事件](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
