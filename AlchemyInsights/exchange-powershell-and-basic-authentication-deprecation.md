---
title: Exchange PowerShell 和基本驗證取代
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015680"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell 和基本驗證取代

如需在不使用基本驗證的情況下連線至 Exchange Online PowerShell 方法的相關最新資訊，請 [移至此處](https://aka.ms/psbasicauth)。

請注意，您的用戶端電腦仍需啟用基本驗證。
新版 PowerShell V2 模組會使用新式驗證來建立啟用所有 REST 基礎 V2 Cmdlet 的連線。 除了 V2 Cmdlet 以外，它也可讓您存取需要建立遠端 PowerShell 工作階段的舊版遠端 PowerShell (RPS) Cmdlets。 即使模組使用新式驗證機制來驗證服務，在 Windows 電腦上建立 RPS 工作階段需要在用戶端電腦上啟用 WinRM 基本驗證。 WinRM 基本驗證管線是用來傳輸新式驗證權杖。 如果在用戶端電腦上停用WinRM 基本驗證，新版 V2 Cmdlet 將繼續運作 (但舊版 RPS 不會)。
