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
ms.openlocfilehash: 51512b29f8d37ce6c39ece5bb704cb01e88e463d
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010245"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>部署適用于 RDS、終端機伺服器或 VDI 的 Microsoft 365 應用程式，供企業共用使用

若要使用遠端桌面服務（RDS）（以前稱為終端機服務）來部署適用于企業的 Microsoft 365 應用程式：
- 您必須具有 Microsoft 365 For Business plan 或 Office 365 方案，其中包含適用于企業的 Microsoft 365 應用程式，例如 Office 365 企業版 E3 或企業版 E5。
   > [!NOTE] 
   > Microsoft 365 應用程式與 Microsoft 365 商務版的 Standard 方案不包含適用于企業的 Microsoft 365 應用程式。
- 您必須啟用[共用電腦](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)啟用。

> [!NOTE]
> 您也可以下載並執行[Microsoft 支援及修復](https://aka.ms/SaRA_OfficeSCA_M365Portal)小幫手，以在共用電腦啟用模式中安裝適用于企業的 Microsoft 365 應用程式。

如需有關使用 Office 部署工具自訂安裝之先決條件、安裝程式指示及指導方針的詳細資訊，請參閱[使用遠端桌面服務部署 Microsoft 365 應用程式（適用于企業](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)）。

若要修正與共享電腦啟用相關的錯誤：
- 請參閱[疑難排解 Microsoft 365 應用程式的共用電腦啟用問題（適用于企業](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)）。
- 請參閱[重設 Microsoft 365 Apps 企業版啟用狀態](https://go.microsoft.com/fwlink/?linkid=2109218)。

如果您想要在 Microsoft 365 系統管理中心（***使用預設安裝設定***）的 RDS 上安裝 Microsoft 365 應用程式，請使用下列步驟：

1.    檢查您擁有的訂閱。 [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    如有必要，請切換至不同的訂閱。 [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    如果已使用任何其他 Microsoft 訂閱在 RDS 伺服器上安裝 Office，請將其卸載。 例如，移至 [**控制台** > ] 中的 [**卸載程式**]。 如果您正在執行問題，請使用[Microsoft 支援和修復](https://aka.ms/SARA-OfficeUninstall-Alchemy)小幫手卸載。
4.    在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並[安裝適用于企業的 microsoft 365 應用程式](https://portal.office.com/OLS/MySoftware.aspx)。
5.    安裝 Office 後，***請勿開啟或登入***任何 office 應用程式。
6.    在 RDS 伺服器上，遵循下列步驟以編輯登錄以啟用共用電腦啟用：
   1. 以滑鼠右鍵按一下螢幕左下角的 [Windows] 按鈕，然後選取 [**執行**]。 在 [開啟] 方塊中輸入**regedit**，然後選取 **[確定]**。
   2. 當系統提示允許登錄編輯程式對您的裝置進行變更時，請選取 **[是]** 。
   3. 在 [登錄編輯程式] 的 [\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.] 底下，新增**SharedComputerLicensing**的設定為 HKEY_LOCAL_MACHINE 1 的字串值。
   4. 在 RDS 伺服器上，以使用者身分登***入***，並[確認已針對 enterprise 的 Microsoft 365 應用程式啟用共用電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

