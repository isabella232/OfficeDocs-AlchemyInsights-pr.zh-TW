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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/01/2021
ms.locfileid: "60040997"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>在 RDS、終端機或 VDI 上部署 Microsoft 365 Apps 企業版以供共用使用

若要使用遠端桌面服務 (RDS) （以前稱為終端機服務）部署 Microsoft 365 Apps，您必須：

- 如果您執行的是舊版本的 Windows，請使用簡易修正程式啟用 TLS 1.2 (例如 Windows 7 SP1，Windows Server 2008 R2) 。 若要輕鬆修正及詳細資訊，請參閱[Update to 啟用 tls 1.1 和 tls 1.2 做為 WinHTTP 中 Windows 中的預設安全通訊協定](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)。 
- 的計畫包含 (先前 Office 365 加) 的 Microsoft 365 Apps 企業版。 例如，Office 365 E3 或 Microsoft 365 E5 或任何包含 Project 或 Visio 的桌上出版本的計畫，例如 Project 方案3或 Visio 方案2或 Microsoft 365 商務進階版計畫，其也包括 Microsoft 365 Apps 商務版。
- 啟用共用電腦啟用。 如需詳細資訊，請參閱[Microsoft 365 Apps 的共用電腦啟用](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)。

**附注**：若要在共用電腦啟用模式中安裝 Microsoft 365 Apps，請下載並執行 [Microsoft 支援及修復小幫手](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds)。 如需有關使用 Office 部署工具來自訂安裝之先決條件、安裝指示及指導方針的詳細資訊，請參閱[使用遠端桌面服務部署 Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)。

若要修正與共享電腦啟用相關的錯誤，請參閱：

- [疑難排解 Microsoft 365 Apps 的共用電腦啟用問題](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [重設 Microsoft 365 Apps for Enterprise 啟用狀態](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

如果您想要從 Microsoft 365 系統管理中心上的 Microsoft 365 Apps 上安裝 RDS，使用預設安裝設定，請遵循下列步驟：

1. 請檢查您所擁有的 Microsoft 365 方案。 如需詳細資訊，請參閱 [我有哪些訂閱？](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)。

1. 如有必要，請切換至不同的 Microsoft 365 計畫。 如需詳細資訊，請參閱 [升級至其他計畫](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)。

1. 如果已使用任何其他不相容的計畫在 RDS 伺服器上安裝 Microsoft 365 Apps，請移至 [**控制台**] 中的 [  >  **卸載程式**]。 如果遇到問題，請下載[Microsoft 支援及修復小幫手](https://aka.ms/SARA-OfficeUninstall-Alchemy)以進行卸載。

1. 在 RDS 伺服器上，使用您的系統管理員帳戶登入 Microsoft 365 系統管理中心，並[安裝 Office](https://portal.office.com/OLS/MySoftware.aspx)。

   安裝 Office 後，請勿開啟或登入任何 Office 應用程式。

1. 在 RDS 伺服器上，編輯登錄以啟用共用電腦啟用：

   1. 在畫面左下角的 [Windows] 按鈕上按一下滑鼠右鍵，然後選取 [**執行**]。 在 [開啟] 方塊中輸入 **regedit**，然後選取 **[確定]**。

   1. 當系統提示您是否允許登錄編輯程式對裝置進行變更時，請選取 **[是]**。

   1. 在 [登錄編輯程式] 的 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \ Office \ClickToRun\Configuration] 底下，新增 **SharedComputerLicensing** 設定為 **1** 的字串值。

1. 在 RDS 伺服器上，以使用者身分登入，並確認已為 Microsoft 365 Apps 啟用共用電腦啟用。 

   如需詳細資訊，請參閱[確認已為 Microsoft 365 Apps 啟用共用電腦啟用](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)。