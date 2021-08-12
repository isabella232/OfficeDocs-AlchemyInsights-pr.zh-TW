---
title: 不顯示敏感度標籤
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061423"
---
# <a name="sensitivity-labels-not-appearing"></a>不顯示敏感度標籤

敏感度標籤可讓您分類並協助保護您的敏感內容。 您可以在 Microsoft 365 合規性中心、Microsoft 365 安全性中心或 Microsoft 365 安全性 & 規範中心的分類 > 敏感度標籤上建立這些功能。 若要深入瞭解這項功能，請參閱 [敏感度標籤簡介](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)。

如果您已設定靈敏度標籤，但未出現在 Microsoft 365 應用程式中，請檢查下列各項：

- 確認敏感度標籤已 [發佈](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) 至您想要的使用者和群組。

- 確認使用者正在使用支援敏感度標籤的應用程式-請參閱 [檔中的靈敏度標籤](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)。

- 如果您要 [遷移 Azure 資訊保護標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)，請注意 [這裡](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)所列的考慮。

- 資料遺失防護 (DLP) 支援：目前，只有保留標籤可以作為 DLP 原則中的條件使用。  無法使用 DLP 原則中的靈敏度標籤，但我們正在處理。

- 在敏感度標籤上啟用加密時，您可以選擇：
    - 立即指派權限
    - 讓使用者指派權限


如需可能問題的詳細資訊，請參閱 [敏感性標籤的已知問題](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)。