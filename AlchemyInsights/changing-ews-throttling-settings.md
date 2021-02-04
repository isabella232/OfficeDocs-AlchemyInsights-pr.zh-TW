---
title: 變更 EWS 節流設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075888"
---
# <a name="changing-ews-throttling-settings"></a>變更 EWS 節流設定

請執行我們的自動測試，讓您在移轉期間修改 EWS 節流原則。 請注意，即使在執行這項作業之後，EWS 匯入仍會限制為每個信箱 150MB，每 5 分鐘一次；若要達到更高的移轉輸送速度，請同時移轉更多使用者。

請注意，EWS 節流原則變更對下列移轉類型 (使用 Microsoft 工具) 沒有任何影響：混合式、完全移轉/分段 (RPC/HTTP)、IMAP、G Suite、公用資料夾或 PST 匯入服務。