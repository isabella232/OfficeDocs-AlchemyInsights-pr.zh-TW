---
title: 用於 Windows 虛擬桌面的服務診斷工具
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052377"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>用於 Windows 虛擬桌面的服務診斷工具

Windows 虛擬桌面 (WVD) 提供了可讓系統管理員透過單一介面識別錯誤的診斷工具。 當被指派 WVD 角色的人員使用 WVD 時，此工具會記錄診斷相關資訊。 每個記錄都包含有關活動中涉及的 WVD 角色之資訊、工作階段期間出現的錯誤訊息以及有關租用戶和使用者的資訊。 Azure 記錄分析可以設定為捕獲診斷工具所建立的活動記錄。 方法如下：

1. 使用 [Azure 入口網站](https://go.microsoft.com/fwlink/?linkid=2129500)或 [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501) 建立記錄分析工作區。
1. [將 Windows 電腦連線至 Azure 監視器](https://go.microsoft.com/fwlink/?linkid=2129913). 取得工作區識別碼和工作區主索引鍵。 設定精靈需要此資訊來正確設定代理程式並確定它可以與 Azure 監視器通訊。
1. [將診斷資料推送至工作區](https://go.microsoft.com/fwlink/?linkid=2128284)。 您可以將 WVD 租用戶中的診斷資料推送至工作區的記錄分析。
1. [識別及診斷](https://go.microsoft.com/fwlink/?linkid=2128338) 與 WVD 相關的內部或外部問題。

若要深入瞭解如何設定 WVD 的服務診斷工具，請參閱 [Use Log Analytics for the diagnostics 功能](https://go.microsoft.com/fwlink/?linkid=2128084)。
