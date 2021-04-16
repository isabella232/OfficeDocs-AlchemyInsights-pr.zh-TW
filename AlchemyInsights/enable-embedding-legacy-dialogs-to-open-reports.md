---
title: 啟用內嵌舊版對話方塊以開啟報告
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814255"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>啟用內嵌舊版對話方塊以開啟報告

**徵狀**

使用者無法開啟報告。 「發生錯誤。 如需詳細資訊，請查看技術詳細資料。」

**原因**

在 UCI 中無法載入報告，出現錯誤：「表單描述項為 Null 或未定義」。 UCI 中的報告仍然需要舊版對話方塊，因此客戶的系統必須啟用 *allowlegacydialogsembedding*。

**解決方案**

1. 移至 **[設定] > [管理] > [系統設定] > [一般] 索引標籤**。

2. 將「在整合介面瀏覽器用戶端中，啟用某些舊版對話方塊的嵌入」設定為 **是**。
