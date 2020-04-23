---
title: 1554 Winsock 錯誤10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766160"
---
# <a name="winsock-error-10061"></a>Winsock 錯誤10061

此錯誤碼表示 Microsoft 無法與目標主機建立 TCP 通訊端（連接）。 這種錯誤最可能的原因是防火牆設定的問題。 若要修正此問題，請檢查這些設定：

- 使用[Microsoft 365 URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊，確認您的防火牆設定

- 如果錯誤是 Exchange Online Protection （EOP）特有的，您就應該先前會收到[Exchange Online PROTECTION IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更通知。

- 確認網際網路服務提供者（ISP）未阻擋埠。

- 驗證連接器中的智慧主機和目標伺服器設定。

請注意，Microsoft 365 不會以這種方式封鎖*傳入*的連線。
