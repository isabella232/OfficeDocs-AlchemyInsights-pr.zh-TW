---
title: 修正 Microsoft 365 的應用程式很抱歉，出現暫時性的伺服器問題訊息
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021587"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>修正 Microsoft 365 應用程式「對不起，我們有暫時的伺服器問題」訊息

如果您收到這封郵件，請嘗試下列步驟：

1. 檢查您的防火牆、防毒軟體及 proxy 設定，以確認他們不會封鎖 Microsoft 365 應用程式的網際網路存取。 請參閱 [URLs 及 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 移至 [**開始**  >  **執行**]，然後輸入 **services.msc**。 請確定下列服務都在執行中：
    - 網路連線裝置自動設定
    - 網路清單服務
    - 網路位置知曉
    - Windows 事件記錄檔

如果其中一項服務未執行，請嘗試啟動它。 如果您在啟動服務時發生問題，請以較高的權限開啟命令提示字元，以執行下列命令：

**sfc/scannow**

完成此命令後，請重新開機電腦。

如需詳細資訊，請參閱 ["對不起，我們無法連線到您的帳戶。啟動時，請稍後再試一次] 錯誤](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。