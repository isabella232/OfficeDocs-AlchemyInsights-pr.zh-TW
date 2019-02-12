---
title: 在終端機伺服器-未授權上安裝 office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918965"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="ca0cb-102">在終端機伺服器上安裝 Office</span><span class="sxs-lookup"><span data-stu-id="ca0cb-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="ca0cb-103">部署 Office 365 ProPlus 使用遠端桌面服務 (RDS) 的 Windows 伺服器上，原先稱為終端機服務：</span><span class="sxs-lookup"><span data-stu-id="ca0cb-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="ca0cb-p101">您必須具備包含 Office 365 ProPlus，例如 Office 365 企業版 E3 或企業 E5 的 Office 365 計劃。Office 365 企業版及 Office 365 企業進階版計劃不包含 Office 365 ProPlus。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="ca0cb-106">您需要啟用[共用的電腦啟用](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="ca0cb-107">如果您想要安裝 Office 365 ProPlus RDS 上從 Office 365 入口網站 \* **以使用預設的安裝設定** \*，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="ca0cb-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="ca0cb-p102">檢查您有哪些 Office 365 計劃。[了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="ca0cb-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="ca0cb-p103">如果需要，切換至不同的 Office 365 計劃。[了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="ca0cb-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="ca0cb-p104">如果使用任何其他 Office 365 計劃的 RDS 伺服器上已安裝 Office，請將它解除安裝。例如，依移至 [控制台]\>解除安裝程式。解除安裝使用[Microsoft 技術支援人員及復原小幫手]](https://aka.ms/SARA-OfficeUninstall-Alchemy)如果您正在執行發生問題。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="ca0cb-115">RDS 伺服器上，登入您的系統管理員帳戶和[安裝 Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)與 Office 365 入口網站。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="ca0cb-116">安裝 Office 之後，\* **不開啟或登入** \* 任何 Office 應用程式。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="ca0cb-117">RDS 伺服器上啟用共用的電腦啟用編輯登錄依照下列步驟：</span><span class="sxs-lookup"><span data-stu-id="ca0cb-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="ca0cb-p105">以滑鼠右鍵按一下您的螢幕左上角的 [Windows] 按鈕，並選取 [執行]。在 [開啟] 方塊中輸入**regedit**，，然後選取 [確定]。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="ca0cb-120">選取 [是] 以允許登錄編輯程式中出現提示時變更您的裝置。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="ca0cb-121">在登錄編輯程式中，使用設定為 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下新增**SharedComputerLicensing**的字串值。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="ca0cb-122">RDS 伺服器上 \* **以使用者身分登入** \* 並[確認已啟用共用的電腦啟用 Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="ca0cb-123">如需必要條件、 安裝指示和指引自訂安裝使用 Office 部署工具的詳細資訊，請參閱[部署 Office 365 ProPlus 使用遠端桌面服務](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="ca0cb-124">若要修正與共用的電腦啟動相關的錯誤，請參閱[共用的電腦啟用 Office 365 proplus 的疑難排解問題](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="ca0cb-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

