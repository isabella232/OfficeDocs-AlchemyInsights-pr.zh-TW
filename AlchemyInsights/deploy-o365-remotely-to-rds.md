---
title: 部署適用于 RDS、終端機伺服器或 VDI 的 Microsoft 365 應用程式，供企業共用使用
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507577"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="98b61-102">部署適用于 RDS、終端機伺服器或 VDI 的 Microsoft 365 應用程式，供企業共用使用</span><span class="sxs-lookup"><span data-stu-id="98b61-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="98b61-103">若要使用遠端桌面服務（RDS）（以前稱為終端機服務）來部署適用于企業的 Microsoft 365 應用程式：</span><span class="sxs-lookup"><span data-stu-id="98b61-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="98b61-104">您必須具有 Microsoft 365 For Business plan 或 Office 365 方案，其中包含適用于企業的 Microsoft 365 應用程式，例如 Office 365 企業版 E3 或企業版 E5。</span><span class="sxs-lookup"><span data-stu-id="98b61-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="98b61-105">Microsoft 365 應用程式與 Microsoft 365 商務版的 Standard 方案不包含適用于企業的 Microsoft 365 應用程式。</span><span class="sxs-lookup"><span data-stu-id="98b61-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="98b61-106">您必須啟用[共用電腦](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)啟用。</span><span class="sxs-lookup"><span data-stu-id="98b61-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="98b61-107">您也可以下載並執行[Microsoft 支援及修復](https://aka.ms/SaRA_OfficeSCA_M365Portal)小幫手，以在共用電腦啟用模式中安裝適用于企業的 Microsoft 365 應用程式。</span><span class="sxs-lookup"><span data-stu-id="98b61-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="98b61-108">如需有關使用 Office 部署工具自訂安裝之先決條件、安裝程式指示及指導方針的詳細資訊，請參閱[使用遠端桌面服務部署 Microsoft 365 應用程式（適用于企業](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)）。</span><span class="sxs-lookup"><span data-stu-id="98b61-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="98b61-109">若要修正與共享電腦啟用相關的錯誤：</span><span class="sxs-lookup"><span data-stu-id="98b61-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="98b61-110">請參閱[疑難排解 Microsoft 365 應用程式的共用電腦啟用問題（適用于企業](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)）。</span><span class="sxs-lookup"><span data-stu-id="98b61-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="98b61-111">請參閱[重設 Microsoft 365 Apps 企業版啟用狀態](https://go.microsoft.com/fwlink/?linkid=2109218)。</span><span class="sxs-lookup"><span data-stu-id="98b61-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="98b61-112">如果您想要在 Microsoft 365 系統管理中心（***使用預設安裝設定***）的 RDS 上安裝 Microsoft 365 應用程式，請使用下列步驟：</span><span class="sxs-lookup"><span data-stu-id="98b61-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="98b61-113">檢查您擁有的訂閱。</span><span class="sxs-lookup"><span data-stu-id="98b61-113">Check what subscription you have.</span></span> <span data-ttu-id="98b61-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="98b61-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="98b61-115">如有必要，請切換至不同的訂閱。</span><span class="sxs-lookup"><span data-stu-id="98b61-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="98b61-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="98b61-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="98b61-117">如果已使用任何其他 Microsoft 訂閱在 RDS 伺服器上安裝 Office，請將其卸載。</span><span class="sxs-lookup"><span data-stu-id="98b61-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="98b61-118">例如，移至 [**控制台**] 中的 [  >  **卸載程式**]。</span><span class="sxs-lookup"><span data-stu-id="98b61-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="98b61-119">如果您正在執行問題，請使用[Microsoft 支援和修復](https://aka.ms/SARA-OfficeUninstall-Alchemy)小幫手卸載。</span><span class="sxs-lookup"><span data-stu-id="98b61-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="98b61-120">在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並[安裝適用于企業的 microsoft 365 應用程式](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="98b61-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="98b61-121">安裝 Office 後，***請勿開啟或登入***任何 office 應用程式。</span><span class="sxs-lookup"><span data-stu-id="98b61-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="98b61-122">在 RDS 伺服器上，遵循下列步驟以編輯登錄以啟用共用電腦啟用：</span><span class="sxs-lookup"><span data-stu-id="98b61-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="98b61-123">以滑鼠右鍵按一下螢幕左下角的 [Windows] 按鈕，然後選取 [**執行**]。</span><span class="sxs-lookup"><span data-stu-id="98b61-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="98b61-124">在 [開啟] 方塊中輸入**regedit**，然後選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="98b61-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="98b61-125">當系統提示允許登錄編輯程式對您的裝置進行變更時，請選取 **[是]** 。</span><span class="sxs-lookup"><span data-stu-id="98b61-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="98b61-126">在 [登錄編輯程式] 的 [\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.] 底下，新增**SharedComputerLicensing**的設定為 HKEY_LOCAL_MACHINE 1 的字串值。</span><span class="sxs-lookup"><span data-stu-id="98b61-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="98b61-127">在 RDS 伺服器上，以使用者身分登***入***，並[確認已針對 enterprise 的 Microsoft 365 應用程式啟用共用電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="98b61-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

