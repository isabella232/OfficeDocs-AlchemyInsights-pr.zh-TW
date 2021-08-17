---
title: 1554 Winsock 錯誤10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083221"
---
# <a name="winsock-error-10061"></a>Winsock 錯誤10061

此錯誤碼表示 Microsoft 無法建立與目標主機的 TCP 通訊端 (連線) 。 這種錯誤最可能的原因是防火牆設定的問題。 若要修正此問題，請檢查這些設定：

- 使用[Microsoft 365 URLs 及 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊，確認您的防火牆設定

- 如果錯誤是 Exchange Online Protection (EOP) 所特有的，您就應該已經收到[Exchange Online Protection IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更。

- 請確認您的網際網路服務提供者 (ISP) 未封鎖埠。

- 驗證連接器中的智慧主機和目標伺服器設定。

請注意，Microsoft 365 不會以這種方式封鎖 *傳入* 的連線。
