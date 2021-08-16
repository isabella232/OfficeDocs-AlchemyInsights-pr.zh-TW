---
title: 在 RDS、終端機或 VDI 上部署 Microsoft 365 Apps 企業版以供共用使用
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031469"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>在 RDS、終端機或 VDI 上部署 Microsoft 365 Apps 企業版以供共用使用

若要使用遠端桌面服務部署 Microsoft 365 Apps 企業版 (RDS) ，以前命名為「終端服務」：

- 您必須具備商務計畫的 Microsoft 365，或包含 Microsoft 365 Apps 企業版的 Office 365 計畫，例如 Office 365 企業版 E3 或 Enterprise E5。
   > [!NOTE]
   > Microsoft 365 Apps 商務版和 Microsoft 365 商務標準版方案不包含 Microsoft 365 Apps 企業版。
- 您必須啟用 [共用電腦](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)啟用。

> [!NOTE]
> 您也可以下載並執行[Microsoft 支援及修復小幫手](https://aka.ms/SaRA_OfficeSCA_M365Portal)，以在共用電腦啟用模式中安裝 Microsoft 365 Apps 企業版。

如需使用 Office 部署工具，針對自訂安裝的必要條件、安裝指示及指導方針的詳細資訊，請參閱[使用遠端桌面服務部署 Microsoft 365 Apps 企業版](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)。

若要修正與共享電腦啟用相關的錯誤：

- 請參閱[疑難排解 Microsoft 365 Apps 企業版的共用電腦啟用問題](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)。
- 請參閱[重設 Microsoft 365 Apps 企業版啟用狀態](https://go.microsoft.com/fwlink/?linkid=2109218)。

如果您想要從 Microsoft 365 系統管理中心上的 Microsoft 365 Apps 企業版上安裝 RDS，使用 ***預設安裝設定***，請使用下列步驟：

1. 檢查您擁有的訂閱。 [Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. 如有必要，請切換至不同的訂閱。 [Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. 如果已使用任何其他 Microsoft 訂閱在 RDS 伺服器上安裝 Office，請將其卸載。 例如，移至 [**控制台**] 中的 [  >  **卸載程式**]。 如果您正在執行問題，請使用[Microsoft 支援及修復小幫手](https://aka.ms/SARA-OfficeUninstall-Alchemy)卸載。
4. 在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並[安裝 Microsoft 365 Apps 企業版](https://portal.office.com/OLS/MySoftware.aspx)。
5. 安裝 Office 後，***請勿開啟或登入*** 任何 Office 應用程式。
6. 在 RDS 伺服器上，遵循下列步驟以編輯登錄以啟用共用電腦啟用：
   1. 以滑鼠右鍵按一下螢幕左下角的 [Windows] 按鈕，然後選取 [**執行**]。 在 [開啟] 方塊中輸入 **regedit**，然後選取 **[確定]**。
   2. 當系統提示允許登錄編輯程式對您的裝置進行變更時，請選取 **[是]** 。
   3. 在登錄編輯程式中，使用 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \ Office \ClickToRun\Configuration. 下的設定為1，新增 **SharedComputerLicensing** 的字串值。
   4. 在 RDS 伺服器上，***以使用者*** 身分登入，並 [確認已為 Microsoft 365 Apps 企業版啟用共用電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。
