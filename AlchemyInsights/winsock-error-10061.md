---
title: 1554 Winsock 錯誤10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e82e90b670235848105636fb2039ed60d3b93c67
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364904"
---
# <a name="winsock-error-10061"></a>Winsock 錯誤10061

此錯誤碼表示 Office 365 無法建立與目標主機的 TCP 通訊端 (連接)。 此錯誤最可能的原因是防火牆設定的問題。 若要修正此問題, 請檢查這些設定:

- 使用[Office 365 url 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊, 確認您的防火牆設定

- 如果錯誤是 Exchange Online Protection (EOP) 所特有, 則您應該曾經收到[Exchange Online PROTECTION IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更通知。

- 確認您的網際網路服務提供者 (ISP) 未封鎖埠。

- 確認連接器中的智慧主機和目標伺服器設定。

請注意, Office 365 不會以這種方式封鎖*傳入*的連線。
