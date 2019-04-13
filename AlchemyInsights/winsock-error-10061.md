---
title: 1554 Winsock 錯誤 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859131"
---
# <a name="winsock-error-10061"></a>Winsock 錯誤 10061

此錯誤代碼表示 Office 365 無法建立與目標主機的 TCP 通訊端 （連線）。 此錯誤最可能的原因是您的防火牆設定問題。 若要修正此問題，請檢查這些設定：

- 確認您的防火牆設定與[Office 365 Url 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊

- 如果此錯誤是特定至 Exchange Online Protection (EOP)，您應該已先前通知到[Exchange Online Protection IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更。

- 確認網際網路服務提供者 (ISP) 不會封鎖連接埠。

- 確認智慧主機 」 和 「 目標伺服器中的設定連接器。

請注意，Office 365 不會封鎖這種方式的*傳入*連線。
