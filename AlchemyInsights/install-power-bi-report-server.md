---
title: 安裝 Power BI 報表伺服器
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
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832085"
---
# <a name="install-power-bi-report-server"></a>安裝 Power BI 報表伺服器

1. 尋找 PowerBIReportServer.exe 的位置，然後啟動安裝程式。

2. 選取 [ **安裝 POWER BI Report Server**]。

3. 選擇要安裝的版本，然後選取 **[下一步]**。

4. 您可以從下拉式清單中選擇 [評估] 或 [開發人員] 版本。  否則，您可以輸入您從 Power BI 服務或大量授權服務中心取得之伺服器的產品金鑰。 如需如何取得產品金鑰的詳細資訊，請參閱「開始之前」一節。 閱讀並同意授權條款及條件，然後選取 **[下一步]**。

5. 您需要有可用的資料庫引擎來儲存報表伺服器資料庫。 選取 **[下一步]** 只安裝報表服務器。

6. 指定報表伺服器的安裝位置。 選取 [ **安裝** ] 以繼續。

7. 成功安裝之後，請選取 [ **設定報表伺服器** ] 以啟動 Reporting Services Configuration Manager。

您不需要在安裝時提供 SQL Server 資料庫引擎伺服器。 安裝之後，您將需要一個設定 Reporting Services 的使用者。

如需詳細資訊： https://docs.microsoft.com/power-bi/report-server/install-report-server
