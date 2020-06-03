---
title: 在終端機伺服器上安裝 office-未授權
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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508619"
---
# <a name="installing-office-on-a-terminal-server"></a>在終端機伺服器上安裝 Office

若要在使用遠端桌面服務（RDS）的 Windows Server （以前稱為終端機服務）上部署 Microsoft 365 應用程式，請執行下列步驟：
  
- 您必須擁有包含 Microsoft 365 應用程式（如 Office 365 企業版 E3 或企業版 E5）的 Microsoft 365 訂閱。 適用于商務用的 Microsoft 365 應用程式和 Microsoft 365 應用程式特優方案不包含適用于企業的 Microsoft 365 應用程式。

- 您需要啟用[共用電腦](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)啟用。

如果您想要在 Microsoft 365 系統管理中心（***使用預設安裝設定***）的 RDS 上安裝 Microsoft 365 應用程式，請使用下列步驟。

> [!TIP]
> 您也可以下載並執行[Microsoft 支援及修復](https://aka.ms/SaRA_OfficeSCA_M365Portal)小幫手，以在共用電腦啟用模式中安裝適用于企業的 Microsoft 365 應用程式。
  
1. 檢查您擁有的 Microsoft 365 訂閱。 [瞭解](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. 如有必要，請切換至不同的 Microsoft 365 訂閱。 [瞭解](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. 如果已使用任何其他 Microsoft 365 訂閱在 RDS 伺服器上安裝 Office，請將其卸載。 例如，移至 [控制台] 中的 [ \> 卸載程式]。 如果您正在執行問題，請使用[Microsoft 支援和修復](https://aka.ms/SARA-OfficeUninstall-Alchemy)小幫手卸載。

4. 在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並[安裝適用于企業的 microsoft 365 應用程式](https://portal.office.com/OLS/MySoftware.aspx)。

5. 安裝 Office 後，***請勿開啟或登入***任何 office 應用程式。

6. 在 RDS 伺服器上，遵循下列步驟以編輯登錄以啟用共用電腦啟用：

1. 在螢幕左下角的 [Windows] 按鈕上按一下滑鼠右鍵，然後選取 [執行]。 在 [開啟] 方塊中輸入**regedit**，然後選取 [確定]。

2. 當系統提示允許登錄編輯程式對您的裝置進行變更時，請選取 [是]。

3. 在 [登錄編輯程式] 的 [\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.] 底下，新增**SharedComputerLicensing**的設定為 HKEY_LOCAL_MACHINE 1 的字串值。

7. 在 RDS 伺服器上，以使用者身分登***入***，並[確認已針對 enterprise 的 Microsoft 365 應用程式啟用共用電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

如需有關使用 Office 部署工具自訂安裝的必要條件、設定指示和指導方針的詳細資訊，請參閱[使用遠端桌面服務部署適用于企業的 Microsoft 365 應用程式](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。
  
若要修正與共享電腦啟用相關的錯誤，請參閱[Microsoft 365 應用程式的共用電腦啟用問題疑難排解](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
  