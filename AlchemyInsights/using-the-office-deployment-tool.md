---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726239"
---
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具（ODT）

您可以使用 Office 部署工具（ODT）來部署 Office 365 版本的 Office。 Office 部署工具（setup.exe）會從命令列執行，並使用設定 XML 檔案，判斷部署 Office 時要套用的設定。
  
1. 從[Microsoft 下載中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具。

2. 使用[Office 自訂工具（OCT）](https://config.office.com)來選取您的部署喜好設定，並建立設定 XML 檔案。 匯出設定檔，並將它放在本機上 setup.exe 所在的相同資料夾中。

    **附注：** 由於誤設定或 malformatted 的設定檔，通常會發生 Office 安裝問題。 為了避免這類問題，我們建議您使用 Office 自訂工具來建立設定檔。 您也可以將現有的設定檔匯入 Office 自訂工具。

3. 從提升許可權的命令提示字元處，切換至 setup.exe 所在的位置，並以下載模式執行 Office 部署工具，並指定您剛儲存的設定檔。 在此範例中，設定檔命名為 config.xml：
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. 在 [設定模式] 中執行 Office 部署工具，並指定設定檔。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **附注：** 您必須從您要安裝 Office 的用戶端電腦執行此步驟，且您必須具有該電腦的本機系統管理員許可權。

若要深入瞭解使用適用于企業部署案例的 Microsoft 365 應用程式的 Office 部署工具，請參閱[Office 部署工具的概述](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。 如需如何使用 Office 自訂工具的詳細資訊，請參閱[Office 自訂工具一覽](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
