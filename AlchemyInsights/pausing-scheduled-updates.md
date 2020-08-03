---
title: 暫停排定的更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530585"
---
# <a name="pausing-scheduled-updates"></a>暫停排定的更新

發出 [暫停] 命令時，裝置在您下次登入 Intune 之前，不會處理命令。 因此，您的裝置可能：

- 在簽入前已安裝排定的更新。
- 在您發出 [暫停] 命令時已關閉電源。 在此情況下，當裝置電源開啟時，他們可能會在簽入前先下載並安裝排定的更新。