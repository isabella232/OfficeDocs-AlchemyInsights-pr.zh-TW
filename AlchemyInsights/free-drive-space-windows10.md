---
title: 在 Windows 10 中釋放磁碟機空間
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928072"
---
# <a name="free-up-drive-space-in-windows-10"></a>在 Windows 10 中釋放磁碟機空間

以下是在 Windows 10 中釋放磁碟機空間的兩種選項：

- 在 Windows 10 中釋放磁碟機空間。
- 使用外部存放裝置釋放 Windows 10 更新的空間。

如果使用 [磁碟清理] 後，磁碟空間仍然不足，您的 Temp 資料夾可能快速填滿 Microsoft Store 所使用的應用程式 (.appx) 檔案。 若要修正此問題，請重設 Microsoft Store、清除 Microsoft Store 快取，然後執行 Windows Update 疑難排解員。 執行這些步驟之前，請確定 Microsoft Store 已關閉。

**步驟 1：重設 Microsoft Store**

**請注意** 這會永久刪除裝置上的應用程式資料，包括您的喜好設定和登入詳細資料。

1. 選取 **[開始]** > **[設定]** > **[應用程式]** > **[應用程式與功能]**。

1. 在應用程式清單中，尋找並選取 Microsoft Store。

1. 選取 **[進階選項]**。

1. 向下捲動並選取 **[重設]**，然後選取 **[確認重設]**。

**步驟 2：清除 Microsoft Store 快取**

1. 按下 Windows 標誌鍵+R，開啟 [執行] 對話方塊。

1. 輸入 wsreset.exe，並選取 **[確定]**。

1. 空白命令提示視窗會隨即開啟。 約 10 秒之後，視窗關閉，Windows Store 會自動開啟。

**步驟 3：重設 Windows Update**

1. 選取 **[開始]** > **[設定]** > **[更新與安全性]** > **[疑難排解]**。

1. 向下捲動並選取 **[Windows Update]**，然後選取 **[執行疑難排解員]**。

1. 將電腦重新開機，並檢查您是否仍遇到問題。

