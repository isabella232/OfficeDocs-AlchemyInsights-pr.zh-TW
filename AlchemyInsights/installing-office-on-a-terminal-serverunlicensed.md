---
title: 終端機伺服器-未經授權上安裝 office
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205400"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8d25e-102">終端機伺服器上安裝 Office</span><span class="sxs-lookup"><span data-stu-id="8d25e-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8d25e-103">部署 Office 365 專業增強版使用遠端桌面服務 (RDS) 的 Windows 伺服器上，以前稱為終端機服務：</span><span class="sxs-lookup"><span data-stu-id="8d25e-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8d25e-104">您必須擁有 Office 365 方案包含 Office 365 專業增強版，例如 Office 365 企業版 E3 或企業版 E5。</span><span class="sxs-lookup"><span data-stu-id="8d25e-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8d25e-105">Office 365 商務版和 Office 365 商務進階版方案並未包含 Office 365 專業增強版。</span><span class="sxs-lookup"><span data-stu-id="8d25e-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="8d25e-106">您要啟用[共用的電腦啟用](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="8d25e-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="8d25e-107">如果您想要安裝 Office 365 專業增強版上從 Microsoft 365 系統管理中心中，***其使用預設安裝的設定***，RDS 使用下列步驟。</span><span class="sxs-lookup"><span data-stu-id="8d25e-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="8d25e-108">您也可以下載並執行[Microsoft 支援及修復小幫手](https://aka.ms/SaRA_OfficeSCA_M365Portal)來共用的電腦啟用模式中安裝 Office 365 專業增強版。</span><span class="sxs-lookup"><span data-stu-id="8d25e-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="8d25e-109">請檢查您有哪些 Office 365 計劃。</span><span class="sxs-lookup"><span data-stu-id="8d25e-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="8d25e-110">了解如何</span><span class="sxs-lookup"><span data-stu-id="8d25e-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8d25e-111">如果有需要時，切換至不同的 Office 365 計劃。</span><span class="sxs-lookup"><span data-stu-id="8d25e-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="8d25e-112">了解如何</span><span class="sxs-lookup"><span data-stu-id="8d25e-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="8d25e-113">如果使用任何其他 Office 365 計劃在 RDS 伺服器上已安裝 Office，請將它解除安裝。</span><span class="sxs-lookup"><span data-stu-id="8d25e-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="8d25e-114">例如，可以移至 [控制台]\>解除安裝程式。</span><span class="sxs-lookup"><span data-stu-id="8d25e-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8d25e-115">解除安裝使用[Microsoft 的支援及修復小幫手](https://aka.ms/SARA-OfficeUninstall-Alchemy)，如果您正在執行發生問題。</span><span class="sxs-lookup"><span data-stu-id="8d25e-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8d25e-116">在 RDS 伺服器上，登入與您的系統管理員帳戶和[安裝 Office 365 專業增強版](https://portal.office.com/OLS/MySoftware.aspx)的 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="8d25e-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8d25e-117">安裝 Office 之後，***不要開啟或登入***任何 Office 應用程式。</span><span class="sxs-lookup"><span data-stu-id="8d25e-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="8d25e-118">在 RDS 伺服器上，啟用共用的電腦啟用編輯登錄遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="8d25e-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8d25e-119">以滑鼠右鍵按一下您的螢幕左上角的 [Windows] 按鈕，選取 [執行]。</span><span class="sxs-lookup"><span data-stu-id="8d25e-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8d25e-120">在 [開啟] 方塊中，輸入**regedit**，，然後選取 [確定]。</span><span class="sxs-lookup"><span data-stu-id="8d25e-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8d25e-121">選取 [是] 以允許登錄編輯程式出現提示時若要變更您的裝置。</span><span class="sxs-lookup"><span data-stu-id="8d25e-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8d25e-122">在登錄編輯程式中，使用設定為 1 下 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 新增**SharedComputerLicensing**的字串值。</span><span class="sxs-lookup"><span data-stu-id="8d25e-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8d25e-123">在 RDS 伺服器上，***以使用者身分登入***並[確認 Office 365 專業增強版已啟用共用的電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="8d25e-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="8d25e-124">如需必要條件、 安裝指示和指引自訂安裝使用 Office 部署工具的詳細資訊，請參閱[部署 Office 365 專業增強版使用遠端桌面服務](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="8d25e-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="8d25e-125">若要修正錯誤相關的共用的電腦啟用，請參閱[Office 365 專業增強版的共用的電腦啟用的疑難排解問題](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="8d25e-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  