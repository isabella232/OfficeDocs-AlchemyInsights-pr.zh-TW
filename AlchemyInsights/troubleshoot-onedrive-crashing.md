---
title: 疑難排解 OneDrive 當機問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826190"
---
# <a name="troubleshoot-onedrive-crashes"></a>疑難排解 OneDrive 當機問題

如果 OneDrive 重複當機，請嘗試下列疑難排解步驟：

**確定是否設定登錄機碼：**

1. 使用 [登錄編輯程式]，並瀏覽至 HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. 如果有 DisableFileSyncNGSC 且設定為 1，請開啟機碼並將值變更為 0。
3. 移至 [開始] 手動啟動 OneDrive ![按 Windows 鍵](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)，在 [搜尋] 方塊中輸入 OneDrive，然後按一下 OneDrive 傳統型應用程式。

**重設 OneDrive：**

附註：

- 重設 OneDrive 會中斷所有現有的同步處理連線 (如果有設定的話，包含您個人的 OneDrive)。
- 重設電腦上的 OneDrive 並不會遺失檔案或資料。

**重設 OneDrive：**

1. 按下 Windows 鍵和 R 開啟 [執行] 對話方塊。
2. 輸入 %localappdata%\Microsoft\OneDrive\onedrive.exe /reset，然後按下 [確定]。 會短暫出現一個 [命令] 視窗。
3. 移至 [開始] 手動啟動 OneDrive ![按 Windows 鍵](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)，在 [搜尋] 方塊中輸入 OneDrive，然後按一下 OneDrive 傳統型應用程式。

附註：

- 如果您在重設前已選擇只同步處理部分的資料夾，您會需要在同步處理完成之後再次設定。 如需詳細資訊，請閱讀 [選擇要同步處理到電腦的 OneDrive 資料夾](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 。
- 您需要為個人 OneDrive 和商務用 OneDrive 完成此步驟。