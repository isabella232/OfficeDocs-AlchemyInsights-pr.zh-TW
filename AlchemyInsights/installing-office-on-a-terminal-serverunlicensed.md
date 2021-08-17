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
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055149"
---
# <a name="installing-office-on-a-terminal-server"></a>在終端機伺服器上安裝 Office

若要使用遠端桌面服務在 Windows 伺服器上部署 Microsoft 365 Apps 企業版 (RDS) （以前稱為終端機服務）：
  
- 您必須擁有包含 Microsoft 365 Apps 企業版的 Microsoft 365 訂閱，例如 Office 365 企業版 E3 或 Enterprise E5。 進階版方案的 Microsoft 365 Apps 商務版和 Microsoft 365 Apps 商務版不包括 Microsoft 365 Apps 企業版。

- 您需要啟用 [共用電腦](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)啟用。

如果您想要從 Microsoft 365 系統管理中心上的 Microsoft 365 Apps 企業版上安裝 RDS，使用 ***預設安裝設定***，請使用下列步驟。

> [!TIP]
> 您也可以下載並執行[Microsoft 支援及修復小幫手](https://aka.ms/SaRA_OfficeSCA_M365Portal)，以在共用電腦啟用模式中安裝 Microsoft 365 Apps 企業版。
  
1. 檢查您擁有的 Microsoft 365 訂閱。 [了解做法](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. 如有必要，請切換至不同的 Microsoft 365 訂閱。 [了解做法](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. 如果 Office 已安裝在 RDS 伺服器上使用任何其他 Microsoft 365 訂閱，請將其卸載。 例如，移至 [控制台] 中的 [ \> 卸載程式]。 如果您正在執行問題，請使用[Microsoft 支援及修復小幫手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸載。

4. 在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並[安裝 Microsoft 365 Apps 企業版](https://portal.office.com/OLS/MySoftware.aspx)。

5. 安裝 Office 後，***請勿開啟或登入*** 任何 Office 應用程式。

6. 在 RDS 伺服器上，遵循下列步驟以編輯登錄以啟用共用電腦啟用：

1. 在畫面左下角的 [Windows] 按鈕上按一下滑鼠右鍵，然後選取 [執行]。 在 [開啟] 方塊中輸入 **regedit**，然後選取 [確定]。

2. 當系統提示允許登錄編輯程式對您的裝置進行變更時，請選取 [是]。

3. 在登錄編輯程式中，使用 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \ Office \ClickToRun\Configuration. 下的設定為1，新增 **SharedComputerLicensing** 的字串值。

7. 在 RDS 伺服器上，***以使用者*** 身分登入，並 [確認已為 Microsoft 365 Apps 企業版啟用共用電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

如需有關使用 Office 部署工具自訂安裝的必要條件、設定指示和指導方針的詳細資訊，請參閱[使用遠端桌面服務部署 Microsoft 365 Apps 企業版](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。
  
若要修正與共享電腦啟用相關的錯誤，請參閱[疑難排解 Microsoft 365 Apps 企業版的共用電腦啟用問題](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
  