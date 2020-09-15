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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698853"
---
# <a name="winsock-error-10061"></a>Winsock 錯誤10061

此錯誤碼表示 Microsoft 無法建立與目標主機的 TCP 通訊端 (連線) 。 這種錯誤最可能的原因是防火牆設定的問題。 若要修正此問題，請檢查這些設定：

- 使用[Microsoft 365 URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊，確認您的防火牆設定

- 如果錯誤是 Exchange Online Protection (EOP) 特有的，您就應該先前會收到 [Exchange Online PROTECTION IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更通知。

- 請確認您的網際網路服務提供者 (ISP) 未封鎖埠。

- 驗證連接器中的智慧主機和目標伺服器設定。

請注意，Microsoft 365 不會以這種方式封鎖 *傳入* 的連線。
