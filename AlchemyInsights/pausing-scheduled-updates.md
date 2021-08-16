---
title: 暫停排定的更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 7ea6c56de00a52080c4a8b47eb5eeee37838420a9e979878c10aeb12885a8b99
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010463"
---
# <a name="pausing-scheduled-updates"></a>暫停排定的更新

發出暫停命令時，在裝置下次簽入 Intune 之前，不會處理該命令。因此，您的裝置可能：

- 在簽入前已安裝排定的更新。
- 在您發出暫停命令時已關閉電源。在此情況下，當裝置電源開啟時，它們可能已在簽入前先下載並安裝排定的更新。