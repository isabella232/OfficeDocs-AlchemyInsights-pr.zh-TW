---
title: 在終端機伺服器上安裝 office-未授權
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663108"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="32e6d-102">在終端機伺服器上安裝 Office</span><span class="sxs-lookup"><span data-stu-id="32e6d-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="32e6d-103">若要在使用遠端桌面服務的 Windows Server 上部署 Microsoft 365 應用程式，請 (RDS) （以前稱為終端機服務）：</span><span class="sxs-lookup"><span data-stu-id="32e6d-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="32e6d-104">您必須擁有包含 Microsoft 365 應用程式（如 Office 365 企業版 E3 或企業版 E5）的 Microsoft 365 訂閱。</span><span class="sxs-lookup"><span data-stu-id="32e6d-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="32e6d-105">適用于商務用的 Microsoft 365 應用程式和 Microsoft 365 應用程式特優方案不包含適用于企業的 Microsoft 365 應用程式。</span><span class="sxs-lookup"><span data-stu-id="32e6d-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="32e6d-106">您需要啟用 [共用電腦](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)啟用。</span><span class="sxs-lookup"><span data-stu-id="32e6d-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="32e6d-107">如果您想要在 Microsoft 365 系統管理中心（ ***使用預設安裝設定***）的 RDS 上安裝 Microsoft 365 應用程式，請使用下列步驟。</span><span class="sxs-lookup"><span data-stu-id="32e6d-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="32e6d-108">您也可以下載並執行 [Microsoft 支援及修復](https://aka.ms/SaRA_OfficeSCA_M365Portal) 小幫手，以在共用電腦啟用模式中安裝適用于企業的 Microsoft 365 應用程式。</span><span class="sxs-lookup"><span data-stu-id="32e6d-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="32e6d-109">檢查您擁有的 Microsoft 365 訂閱。</span><span class="sxs-lookup"><span data-stu-id="32e6d-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="32e6d-110">瞭解</span><span class="sxs-lookup"><span data-stu-id="32e6d-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="32e6d-111">如有必要，請切換至不同的 Microsoft 365 訂閱。</span><span class="sxs-lookup"><span data-stu-id="32e6d-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="32e6d-112">瞭解</span><span class="sxs-lookup"><span data-stu-id="32e6d-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="32e6d-113">如果已使用任何其他 Microsoft 365 訂閱在 RDS 伺服器上安裝 Office，請將其卸載。</span><span class="sxs-lookup"><span data-stu-id="32e6d-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="32e6d-114">例如，移至 [控制台] 中的 [ \> 卸載程式]。</span><span class="sxs-lookup"><span data-stu-id="32e6d-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="32e6d-115">如果您正在執行問題，請使用 [Microsoft 支援和修復](https://aka.ms/SARA-OfficeUninstall-Alchemy) 小幫手卸載。</span><span class="sxs-lookup"><span data-stu-id="32e6d-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="32e6d-116">在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並 [安裝適用于企業的 microsoft 365 應用程式](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="32e6d-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="32e6d-117">安裝 Office 後， ***請勿開啟或登入*** 任何 office 應用程式。</span><span class="sxs-lookup"><span data-stu-id="32e6d-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="32e6d-118">在 RDS 伺服器上，遵循下列步驟以編輯登錄以啟用共用電腦啟用：</span><span class="sxs-lookup"><span data-stu-id="32e6d-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="32e6d-119">在螢幕左下角的 [Windows] 按鈕上按一下滑鼠右鍵，然後選取 [執行]。</span><span class="sxs-lookup"><span data-stu-id="32e6d-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="32e6d-120">在 [開啟] 方塊中輸入 **regedit**，然後選取 [確定]。</span><span class="sxs-lookup"><span data-stu-id="32e6d-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="32e6d-121">當系統提示允許登錄編輯程式對您的裝置進行變更時，請選取 [是]。</span><span class="sxs-lookup"><span data-stu-id="32e6d-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="32e6d-122">在 [登錄編輯程式] 的 [\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.] 底下，新增 **SharedComputerLicensing** 的設定為 HKEY_LOCAL_MACHINE 1 的字串值。</span><span class="sxs-lookup"><span data-stu-id="32e6d-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="32e6d-123">在 RDS 伺服器上，以使用者身分登 ***入*** ，並 [確認已針對 enterprise 的 Microsoft 365 應用程式啟用共用電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="32e6d-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="32e6d-124">如需有關使用 Office 部署工具自訂安裝的必要條件、設定指示和指導方針的詳細資訊，請參閱 [使用遠端桌面服務部署適用于企業的 Microsoft 365 應用程式](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。</span><span class="sxs-lookup"><span data-stu-id="32e6d-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="32e6d-125">若要修正與共享電腦啟用相關的錯誤，請參閱 [Microsoft 365 應用程式的共用電腦啟用問題疑難排解](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。</span><span class="sxs-lookup"><span data-stu-id="32e6d-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  