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
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721546"
---
# <a name="pausing-scheduled-updates"></a>暫停排定的更新

發出 [暫停] 命令時，裝置在您下次登入 Intune 之前，不會處理命令。 因此，您的裝置可能：

- 在簽入前已安裝排定的更新。
- 在您發出 [暫停] 命令時已關閉電源。 在此情況下，當裝置電源開啟時，他們可能會在簽入前先下載並安裝排定的更新。