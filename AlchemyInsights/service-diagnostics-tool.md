---
title: 用於 Windows 虛擬桌面的服務診斷工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: e6c20af2c3fc54b203f3bda5c0c0f00faacd92800566bd507867c4e9fe4a23f1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052305"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>用於 Windows 虛擬桌面的服務診斷工具

Windows 虛擬桌面 (WVD) 提供了可讓系統管理員透過單一介面識別錯誤的診斷工具。 當被指派 WVD 角色的人員使用 WVD 時，此工具會記錄診斷相關資訊。 每個記錄都包含有關活動中涉及的 WVD 角色之資訊、工作階段期間出現的錯誤訊息以及有關租用戶和使用者的資訊。 Azure 記錄分析可設定為透過以下步驟擷取診斷工具建立的活動記錄：

1. 使用 [Azure 入口網站](https://go.microsoft.com/fwlink/?linkid=2129500)或 [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501) 建立記錄分析工作區。

1. [將 Windows 電腦連線至 Azure 監視器](https://go.microsoft.com/fwlink/?linkid=2129913). 取得工作區識別碼和工作區主索引鍵。 設定精靈需要此資訊來正確設定代理程式並確定它可以與 Azure 監視器通訊。

1. [將診斷資料推送至工作區](https://go.microsoft.com/fwlink/?linkid=2128284)。 您可以將 WVD 租用戶中的診斷資料推送至工作區的記錄分析。

1. [識別和診斷](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)與 WVD 相關的內部或外部問題。

若要深入了解為 WVD 設定服務診斷工具的資訊，請參閱使用記錄分析進行診斷功能。