---
title: 您的封存信箱快滿了
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950504"
---
# <a name="your-archive-mailbox-is-almost-full"></a>您的封存信箱快滿了

如果使用者收到警告; **您的封存信箱快滿**，或者您需要增加其封存信箱的大小，以下是一些秘訣：

1. 若使用者已獲指派 Exchange Online 方案1，請升級至 **Exchange Online plan 2** 授權，將大小從 50 GB 增加至100GB。
1. 若使用者已被指派下列其中一項： **Exchange Online plan 2** 或 Exchange online plan 1 （包含 exchange online 封存附加元件），請使用下列步驟來啟用自動擴充封存：。
 
    1. [連接至 Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。
    2. 為使用者執行下列 commandlet：  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. 執行下列 commandlet，確認已為使用者啟用此功能：  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

如需詳細資訊，請參閱：

- [ 啟用無限封存-系統管理說明-Microsoft 365 符合性 |Microsoft 檔](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online 限制-服務說明 |Microsoft 檔](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [升級至不同的商務計畫 |Microsoft 檔](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

