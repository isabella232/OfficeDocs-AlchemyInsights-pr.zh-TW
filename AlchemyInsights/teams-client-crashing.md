---
title: Teams 用戶端當機？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030540"
---
# <a name="teams-client-crashing"></a>Teams 用戶端當機？

如果您的 Teams 用戶端當機，請嘗試下列操作：

- 如果您使用的是 Teams 傳統型應用程式，請[確定應用程式已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

- 請確定所有 [Office 365 URL 和位址範圍](https://docs.microsoft.com/microsoftteams/connectivity-issues)皆可存取。

- 使用您的系統管理員帳戶登入，並檢查您的[服務健康情況儀表板](https://docs.microsoft.com/office365/enterprise/view-service-health) (部分機器翻譯)，確認沒有中斷或服務降級。

 - 最後，您可以嘗試清除 Teams 用戶端快取：

    1.  完全關閉 Microsoft Teams 桌面用戶端。 您可以在圖示匣中，以滑鼠右鍵按一下 [Teams]****，然後按一下 [結束]**** 或執行 [工作管理員] 並完全終止程序。

    2.  移至 [檔案總管]，然後輸入 %appdata%\Microsoft\teams。

    3.  在目錄中，您會看到下列幾個資料夾：

         - 在 [應用程式快取]**** 內，移至 [快取]，並刪除 [快取] 位置中的任何檔案：%appdata%\Microsoft\teams\application cache\cache。

        - 在 [Blob_storage]**** 內，刪除所有檔案：%appdata%\Microsoft\teams\blob_storage。

        - 在 [快取]**** 內，刪除所有檔案：%appdata%\Microsoft\teams\Cache。

        - 在 [資料庫]**** 內，刪除所有檔案：%appdata%\Microsoft\teams\databases。

        - 在 [GPUCache]**** 內，刪除所有檔案：%appdata%\Microsoft\teams\GPUcache。

        - 在 [IndexedDB]**** 內，刪除 .db 檔案：%appdata%\Microsoft\teams\IndexedDB。

        - 在 [本機儲存體]**** 內，刪除所有檔案：%appdata%\Microsoft\teams\Local Storage。

        - 最後，在 [tmp]**** 內，刪除任何檔案：%appdata%\Microsoft\teams\tmp。

    4. 重新啟動您的 Teams 用戶端。
