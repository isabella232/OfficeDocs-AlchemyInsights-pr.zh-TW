---
title: '[警示] 索引標籤中遺失的警示'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362366"
---
# <a name="alerts-missing-from-alerts-tab"></a>[警示] 索引標籤中遺失的警示

[ **警示** ] 索引標籤的運作方式取決於您租使用者中的應用程式管理入口網站的設定和啟用的原則。 在應用程式控管中的現成原則也必須啟用，讓信號流向 [ **警示** ] 索引標籤。 

確認已產生警示：

1. 移至應用程式管理 [原則](https://compliance.microsoft.com/m365appprotection?viewid=policies) ，並確認您已建立至少一個作用中或審計原則。

1. 選取原則，然後 seleect 彈出窗格中的 [ **編輯** ]。 

1. 請檢查原則設定，以確認是否應該根據在超過24小時之前所啟動的原則事件產生警示。

如需有關應用程式管理提醒的詳細資訊，請參閱 [開始使用應用程式威脅偵測和修正](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)。