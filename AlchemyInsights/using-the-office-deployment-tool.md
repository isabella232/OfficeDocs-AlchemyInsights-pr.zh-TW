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
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="f9be1-102">使用 Office 部署工具 (ODT)</span><span class="sxs-lookup"><span data-stu-id="f9be1-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="f9be1-103">您可以使用 Office 部署工具 (ODT) 來部署 Office 365 版本的 Office。</span><span class="sxs-lookup"><span data-stu-id="f9be1-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="f9be1-104">Office 部署工具 (setup.exe) 執行從命令列，並使用設定 XML 檔案來決定要部署 Office 時，會套用哪些設定。</span><span class="sxs-lookup"><span data-stu-id="f9be1-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="f9be1-105">從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="f9be1-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="f9be1-106">使用[Office 自訂工具 (OCT)](https://config.office.com)來選取您的部署喜好設定，並建立組態 XML 檔案。</span><span class="sxs-lookup"><span data-stu-id="f9be1-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="f9be1-107">匯出設定檔，並在本機上放在 setup.exe 所在的相同資料夾。</span><span class="sxs-lookup"><span data-stu-id="f9be1-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="f9be1-108">**附註：** Office 安裝問題通常就會發生到期，若要設定錯誤或 malformatted 組態檔。</span><span class="sxs-lookup"><span data-stu-id="f9be1-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="f9be1-109">若要避免這種問題，我們建議您使用 Office 自訂工具來建立組態檔。</span><span class="sxs-lookup"><span data-stu-id="f9be1-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="f9be1-110">您也可以在 Office 自訂工具匯現有設定檔。</span><span class="sxs-lookup"><span data-stu-id="f9be1-110">You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="f9be1-111">從提升權限的命令提示字元處，切換至 setup.exe 所在的位置，以下載模式執行 Office 部署工具並指定您剛儲存的組態檔。</span><span class="sxs-lookup"><span data-stu-id="f9be1-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="f9be1-112">在這個範例中，組態檔名為 Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="f9be1-112">In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="f9be1-113">執行 Office 部署工具以 configure 模式，並指定設定檔。</span><span class="sxs-lookup"><span data-stu-id="f9be1-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="f9be1-114">**附註：** 您必須從用戶端電腦您想要安裝 Office，您必須具備本機系統管理員權限在該電腦上執行此步驟。</span><span class="sxs-lookup"><span data-stu-id="f9be1-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="f9be1-115">若要深入了解 Office 365 專業增強版的部署案例中使用 Office 部署工具的詳細資訊，請參閱[Office 部署工具概觀](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)。</span><span class="sxs-lookup"><span data-stu-id="f9be1-115">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool).</span></span> <span data-ttu-id="f9be1-116">如需如何使用 Office 自訂工具的詳細資訊，請參閱 < <b0>Office 自訂工具概觀</b0>。</span><span class="sxs-lookup"><span data-stu-id="f9be1-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

