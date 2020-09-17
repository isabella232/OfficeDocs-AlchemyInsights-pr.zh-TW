---
title: 啟用內嵌舊版對話方塊以開啟報告
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
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806426"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>啟用內嵌舊版對話方塊以開啟報告

**徵狀**

使用者無法開啟報告。 「發生錯誤。 如需詳細資訊，請查看技術詳細資料。」

**原因**

在 UCI 中無法載入報告，出現錯誤：「表單描述項為 Null 或未定義」。 UCI 中的報告仍然需要舊版對話方塊，因此客戶的系統必須啟用 *allowlegacydialogsembedding*。

**解決方案**

1. 移至 **[設定] > [管理] > [系統設定] > [一般] 索引標籤**。

2. 將「在整合介面瀏覽器用戶端中，啟用某些舊版對話方塊的嵌入」設定為**是**。
