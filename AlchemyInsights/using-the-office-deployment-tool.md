---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423174"
---
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具 (ODT)

您可以使用 Office 部署工具 (ODT) 來部署 Office 365 版本的 Office。 Office 部署工具 (setup.exe) 執行從命令列，並使用設定 XML 檔案來決定要部署 Office 時，會套用哪些設定。
  
1. 從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具。
    
2. 使用[Office 自訂工具 (OCT)](https://config.office.com)來選取您的部署喜好設定，並建立組態 XML 檔案。 匯出設定檔，並在本機上放在 setup.exe 所在的相同資料夾。 
    
    **附註：** Office 安裝問題通常就會發生到期，若要設定錯誤或 malformatted 組態檔。 若要避免這種問題，我們建議您使用 Office 自訂工具來建立組態檔。 您也可以在 Office 自訂工具匯現有設定檔。 
    
3. 從提升權限的命令提示字元處，切換至 setup.exe 所在的位置，以下載模式執行 Office 部署工具並指定您剛儲存的組態檔。 在這個範例中，組態檔名為 Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. 執行 Office 部署工具以 configure 模式，並指定設定檔。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **附註：** 您必須從用戶端電腦您想要安裝 Office，您必須具備本機系統管理員權限在該電腦上執行此步驟。 
    
若要深入了解 Office 365 專業增強版的部署案例中使用 Office 部署工具的詳細資訊，請參閱[Office 部署工具概觀](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。 如需如何使用 Office 自訂工具的詳細資訊，請參閱 < <b0>Office 自訂工具概觀</b0>。
  

