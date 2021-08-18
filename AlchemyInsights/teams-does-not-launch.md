---
title: Teams 無法啟動
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329317"
---
# <a name="teams-doesnt-launch"></a>Teams 無法啟動

如果您嘗試開啟 Microsoft Teams 但從未啟動，請嘗試下列方法：

1. 瀏覽至 **%appdata%\Microsoft\Teams**。
1. 刪除資料夾的內容。
1. 重新啟動電腦，然後嘗試啟動 Teams。

您可能需要重新安裝 Teams。若要重新安裝：

1. 使用 [控制台] 解除安裝 Teams。
1. 瀏覽至 **%appdata%\Microsoft\Teams\Application Cache**。
1. 刪除資料夾的內容。
1. 瀏覽至 **%appdata%\Microsoft\teams\Cache**。
1. 刪除資料夾的內容。
1. 重新啟動電腦，然後下載並安裝 Teams。

如果您想要針對無法登入的特定使用者，在租用戶上執行診斷，請以關鍵字 **TeamsUserUnableToSignIn** 開始新的搜尋，然後按照提示進行。