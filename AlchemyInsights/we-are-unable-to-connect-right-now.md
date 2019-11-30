---
title: 啟用此問題:-我們目前無法連線現在
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628233"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>修正 Office 應用程式 」 我們目前無法連線現在的 「 郵件

如果您收到這封郵件，請嘗試下列作法：

1. 檢查您的防火牆、 防毒軟體，與 proxy 設定，以確認，它們都不會封鎖 Office 相關應用程式的網際網路存取。 請參閱[Office 365 Url 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 移至**開始** > **執行**，然後再類型**services.msc**。 請確認下列服務所有執行中：
    - 網路連線的裝置自動設定
    - 網路清單服務
    - 網路位置認知
    - Windows 事件記錄檔

如果其中一個服務未執行，嘗試啟動它。 如果您有問題，啟動服務，以提高權限的權限開啟命令提示字元中執行下列命令：

**sfc /scannow**

此命令完成之後，重新啟動電腦。

如需詳細資訊，請參閱[「 很抱歉，我們無法連線至您的帳戶。請稍後再試 」 錯誤，當您啟動從 Office 365 的 Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。