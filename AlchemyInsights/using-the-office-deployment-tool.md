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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="208cf-102">使用 Office 部署工具 (ODT)</span><span class="sxs-lookup"><span data-stu-id="208cf-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="208cf-p101">您可以使用 Office 部署工具 (ODT) 來部署 Office 365 的 Office 版本。Office 部署工具 (setup.exe) 從命令列執行，並決定要部署 Office 時套用設定的使用設定 XML 檔案。</span><span class="sxs-lookup"><span data-stu-id="208cf-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="208cf-105">從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="208cf-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="208cf-p102">使用[Office 自訂工具 (OCT)](https://config.office.com)來選取您的部署喜好設定並建立設定 XML 檔案。匯出組態檔並將它從本機 setup.exe 所在的相同資料夾。</span><span class="sxs-lookup"><span data-stu-id="208cf-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="208cf-p103">**附註：** 經常發生問題到期來設定錯誤的 office 安裝或 malformatted 設定檔。若要避免此類問題，我們建議您在建立設定檔使用 「 Office 自訂工具 」。您也可以使用 Office 自訂工具將匯入現有的設定檔。</span><span class="sxs-lookup"><span data-stu-id="208cf-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="208cf-p104">從提升權限的命令提示字元處，切換至 setup.exe 所在的位置並以 download 模式執行 Office 部署工具並指定您剛儲存的設定檔。在本例中為設定檔名為 Configuration.xml：</span><span class="sxs-lookup"><span data-stu-id="208cf-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="208cf-113">執行 Office 部署工具以 configure 模式與指定的設定檔。</span><span class="sxs-lookup"><span data-stu-id="208cf-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="208cf-114">**附註：** 您必須從用戶端電腦您要安裝 Office 與您必須在該電腦上本機系統管理員權限來執行此步驟。</span><span class="sxs-lookup"><span data-stu-id="208cf-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="208cf-p105">若要深入了解 Office 365 ProPlus 的部署案例中使用 Office 部署工具，請參閱[Office 部署工具的概觀](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。如需如何使用 Office 自訂工具的詳細資訊，請參閱 ＜ [Office 自訂工具概觀](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)。</span><span class="sxs-lookup"><span data-stu-id="208cf-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

