---
title: 變更 EWS 節流設定
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968368"
---
# <a name="changing-ews-throttling-settings"></a>變更 EWS 節流設定

請執行我們的自動測試，讓您在移轉期間修改 EWS 節流原則。 請注意，即使在執行這項作業之後，EWS 匯入仍會限制為每個信箱 150MB，每 5 分鐘一次；若要達到更高的移轉輸送速度，請同時移轉更多使用者。

請注意，EWS 節流原則變更對下列移轉類型 (使用 Microsoft 工具) 沒有任何影響：混合式、完全移轉/分段 (RPC/HTTP)、IMAP、G Suite、公用資料夾或 PST 匯入服務。