---
title: Microsoft 365 中的2681攻擊模擬器
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506729"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365 中的攻擊模擬器

- 您是否遺漏攻擊模擬器？ 攻擊模擬器需要**Office 365 高級威脅防護方案2（ATP 方案2）** 或**Office 365 企業版 E5**。 「Office 365 高級威脅防護方案1（ATP 方案1）」、Office 365 企業版 E3 或任何 Microsoft 365 Apps for business 訂閱中**不**包含攻擊模擬器。

- 您用來啟動模擬攻擊的帳戶需要全域系統管理員或安全性管理員許可權，以及多重要素驗證（MFA）。 如需有關攻擊模擬程式需求的詳細資訊，請參閱[本主題](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。

- 關於**強力強制密碼**攻擊模擬的重要事項：

  - 如果目標帳戶已啟用 MFA，且密碼猜測正確，該帳戶將不會顯示為 [已遭破壞] （第二個驗證因素將不完整）。

  - 密碼檔不可超過 10 MB。 每行使用一個密碼，並在清單中的最後一個密碼之後加入一條空白行（回車）。

- **Spear 網路釣魚**附加模擬所需注意的重要事項：

  - 根據設計，您無法為**網路釣魚登入伺服器 URL**提供自訂值。

  - 如果收件者使用「[啟用報告訊息增益集](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)」，將郵件報告為網路釣魚，您可能不會收到郵件的警示（因為這是模擬型攻擊）。

- 報告：模擬的攻擊完成後，您可以按一下 [**攻擊詳細資料**] 以查看報告。

- 如需攻擊模擬器的詳細指示和新功能，請參閱[Microsoft 365 中的攻擊模擬器](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)。
