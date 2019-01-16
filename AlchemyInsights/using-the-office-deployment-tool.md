---
title: 使用 Office 部署工具
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279069"
---
# <a name="using-the-office-deployment-tool-odt"></a>使用 Office 部署工具 (ODT)

您可以使用 Office 部署工具 (ODT) 來部署 Office 365 的 Office 版本。Office 部署工具 (setup.exe) 從命令列執行，並決定要部署 Office 時套用設定的使用設定 XML 檔案。
  
1. 從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具。
    
2. 使用[Office 自訂工具 (OCT)](https://config.office.com)來選取您的部署喜好設定並建立設定 XML 檔案。匯出組態檔並將它從本機 setup.exe 所在的相同資料夾。 
    
    **附註：** 經常發生問題到期來設定錯誤的 office 安裝或 malformatted 設定檔。若要避免此類問題，我們建議您在建立設定檔使用 「 Office 自訂工具 」。您也可以使用 Office 自訂工具將匯入現有的設定檔。 
    
3. 從提升權限的命令提示字元處，切換至 setup.exe 所在的位置並以 download 模式執行 Office 部署工具並指定您剛儲存的設定檔。在本例中為設定檔名為 Configuration.xml：
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. 執行 Office 部署工具以 configure 模式與指定的設定檔。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **附註：** 您必須從用戶端電腦您要安裝 Office 與您必須在該電腦上本機系統管理員權限來執行此步驟。 
    
若要深入了解 Office 365 ProPlus 的部署案例中使用 Office 部署工具，請參閱[Office 部署工具的概觀](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。如需如何使用 Office 自訂工具的詳細資訊，請參閱 ＜ [Office 自訂工具概觀](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。
  

