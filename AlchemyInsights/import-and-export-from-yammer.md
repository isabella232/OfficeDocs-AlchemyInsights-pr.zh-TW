---
title: 從 Yammer 匯入和匯出
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
- "9735"
- "9003224"
ms.openlocfilehash: b365921d3ca64e8ad4bd3891e11add8043b2a903
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329817"
---
# <a name="import-and-export-from-yammer"></a>從 Yammer 匯入和匯出

**匯入**

使用者匯入選項會根據您的 Yammer 網路是[適用於 Microsoft 365 的原生模式](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)與否而有所不同。

- **非原生模式**：可以使用群組設定內的 [從通訊錄新增](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (限制為 100 個使用者) 將使用者匯入到群組，或使用網路系統管理員內的 [大量更新](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)，將使用者匯入到網路。
- **原生模式**：群組成員資格和網路成員資格作業應該從 [Microsoft 365 系統管理入口網站](https://docs.microsoft.com/microsoft-365/admin/add-users)、[Azure AD 入口網站](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)，或是使用另一個 Azure AD 選項執行。 原生模式的網路無法再存取大量更新和其他舊版功能。

    **重要**：Yammer 從未支援匯入來自網路系統管理員的內容，即使資料匯出功能已用於其他網路也一樣。 合作夥伴解決方案或 Yammer REST API 可以重新發佈內容。

**匯出**

[匯出網路系統管理員內的網路資料](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)，允許從 Yammer 網路匯出內容，包括訊息和檔案。 附件可能會非常龐大，且會導致匯出需要大量時間才能完成。 我們建議使用[資料匯出 API](https://developer.yammer.com/docs/data-export-api)，依日或週以區塊匯出使用中網路。 Microsoft 支援服務不會為此目的提供自訂指令碼。

有個別 [GDPR 匯出](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)，匯出個別使用者的內容。