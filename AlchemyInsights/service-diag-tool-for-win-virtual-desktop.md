---
title: Windows 虛擬桌面的服務診斷工具
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665816"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows 虛擬桌面的服務診斷工具

Windows Virtual Desktop (WVD) 提供診斷工具，可讓系統管理員透過單一介面識別錯誤。 此工具會記錄與診斷相關的資訊，每當指派 WVD 角色的人員使用 WVD 時。 每個記錄檔都包含有關活動中所涉及之 WVD 角色的資訊、在會話期間出現的錯誤訊息，以及租使用者和使用者的相關資訊。 Azure 記錄分析可以設定為捕獲診斷工具所建立的活動記錄。 方法如下：

1. 使用 [azure 入口網站](https://go.microsoft.com/fwlink/?linkid=2129500) 或 [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)建立 Log Analytics 工作區。
1. [將 Windows 電腦連線到 Azure 監視器](https://go.microsoft.com/fwlink/?linkid=2129913)。 取得您的工作區的工作區識別碼及主金鑰。 安裝精靈需要此資訊才能正確地設定代理程式，並確保其可以與 Azure 監視器通訊。
1. [將診斷資料推送至您的工作區](https://go.microsoft.com/fwlink/?linkid=2128284)。 您可以將 WVD 租使用者的診斷資料推送至您的工作區的記錄分析。
1. [識別及診斷](https://go.microsoft.com/fwlink/?linkid=2128338) 與 WVD 相關的內部或外部問題。

若要深入瞭解如何設定 WVD 的服務診斷工具，請參閱 [Use Log Analytics for the diagnostics 功能](https://go.microsoft.com/fwlink/?linkid=2128084)。
