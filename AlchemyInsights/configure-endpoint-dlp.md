---
title: 設定端點 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: f29d8476881fb3f93b369c057efed0acdd2169baf956ab43bf3c0ade527e9437
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033521"
---
# <a name="configure-endpoint-dlp"></a>設定端點 DLP

Microsoft 端點 DLP 可讓可以您將 DLP 保護和監視功能延伸到 Windows 10 裝置上的敏感性資訊。 將裝置上線至裝置管理中後，您就可以建立 DLP 原則，在項目上強制執行保護動作。 活動總管可用來監視敏感性項目的活動。 如需詳細資訊，請參閱 [將裝置上線至裝置管理](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)。  

若要開始使用端點 DLP：

- 請確認您擁有適當的 SKU/訂閱授權。 如需詳細資訊，請參閱 [SKU/訂閱授權](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)。
- 檢查啟用裝置管理、存取上線頁面或開啟/關閉裝置監視所需的權限。如需詳細資訊，請參閱[權限](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)。
- 遵循上線裝置程序將裝置上線至裝置管理。 如需詳細資訊，請參閱 [上線裝置](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)。 
- 建立 DLP 原則以保護您的敏感性項目。 如需詳細資訊，請參閱 [端點 DLP 原則案例](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)。

如需有關 Microsoft 端點 DLP，請參閱 [深入了解 Microsoft 365 端點資料外洩防護 (預覽版)](/microsoft-365/compliance/endpoint-dlp-learn-about)。

**如果需要支援，以下是重要資料收集步驟：**

1. 下載 [MDATP 用戶端分析器預覽](https://aka.ms/betamdatpanalyzer)。
1. 使用 cmd 視窗以系統管理員身分執行工具：

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. 當系統提示 [輸入收集追蹤的分鐘數:] 時，輸入執行案例所需的分鐘數。
1. 執行案例。

收集 Zip 檔案輸出，以提供給支援專員。
