---
title: 升級至 macOS 11.6 Big Sur 之後無法新增帳戶
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446721"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>升級至 macOS 11.6 Big Sur 之後無法新增帳戶

升級至 macOS 11.6 之後，您的公司或學校用 OneDrive 帳戶或 OneDrive 個人帳戶可能不會出現在您的帳戶清單中，而且您可能無法從應用程式登入第二個帳戶。

這是與 macOS 11.6 升級相關的新出現問題。 在解決此問題之前，您可以從網頁或行動裝置存取您的 OneDrive 內容。 Microsoft 正與 Apple 合作以還原 OneDrive 功能。

您也可以透過使用 Terminal 手動啟動遺失的 OneDrive 執行個體。 

**注意**：此因應措施僅在重新啟動 OneDrive 之前有效 (電腦重新開機或 OneDrive 應用程式更新)。

如果遺失的執行個體為個人帳戶，請開啟 [Terminal] 並輸入：

`open "/Applications/OneDrive.app" --new --args /client=Personal`

如果遺失的執行個體是工作或學校帳戶，請開啟 [Terminal] 並輸入：

`open "/Applications/OneDrive.app" --new --args /client=Business1`

