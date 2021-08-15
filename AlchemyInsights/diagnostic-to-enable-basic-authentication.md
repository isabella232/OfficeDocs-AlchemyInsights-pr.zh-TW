---
title: 診斷以啟用 Exchange Online 通訊協定的基本驗證
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11392"
- "9006699"
ms.openlocfilehash: 25979df257d0534709f610b4d1547c52aeb269053c3d15a38969f15223b59e04
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993596"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a>診斷以啟用 Exchange Online 通訊協定的基本驗證

透過使用此診斷，您可以為 Exchange Online 通訊協定 (例如 POP3、IMAP4、Exchange ActiveSync、Exchange Web 服務、離線通訊錄、MAPI、RPC 和遠端 PowerShell) 啟用基本驗證，Microsoft 最近可能已為貴組織停用此驗證。 

我們正在透過訊息中心傳送直接通訊，讓租用戶知道他們因為沒有任何使用量，因而已準備好關閉環境中的基本驗證，這可協助保護其環境免受相關安全性風險的影響。