---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 998f914f38fa9d1925f7003e634d7f11550f47da
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365516"
---
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具 (ODT)

您可以使用 Office 部署工具 (ODT) 來部署 Office 365 版本的 Office。 Office 部署工具 (setup.exe) 是從命令列執行, 並使用設定 XML 檔案來決定部署 Office 時要套用的設定。
  
1. 從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版本的 Office 部署工具。

2. 使用[Office 自訂工具 (OCT)](https://config.office.com)來選取您的部署喜好設定, 並建立設定 XML 檔案。 匯出設定檔, 並將它置於 setup.exe 所在的相同資料夾中。

    **附注:** 由於誤設定或 malformatted 設定檔, 通常會發生 Office 安裝問題。 若要避免這類問題, 建議您使用 Office 自訂工具來建立設定檔。 您也可以將現有的設定檔匯入 Office 自訂工具。

3. 從提升許可權的命令提示字元處, 切換到 setup.exe 所在的位置, 並在下載模式中執行 Office 部署工具, 並指定您剛儲存的設定檔。 在此範例中, 設定檔命名為 config.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. 在 [設定] 模式中執行 Office 部署工具, 並指定設定檔。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **附注:** 您必須在要安裝 Office 的用戶端電腦上執行此步驟, 而且必須具有該電腦的本機系統管理員許可權。

若要深入瞭解如何使用 office 部署工具進行 Office 365 專業增強版部署案例, 請參閱[Office 部署工具的總覽](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。 如需如何使用 Office 自訂工具的詳細資訊, 請參閱[Office 自訂工具的總覽](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
