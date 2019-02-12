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
# <a name="installing-office-on-a-terminal-server"></a>在終端機伺服器上安裝 Office

部署 Office 365 ProPlus 使用遠端桌面服務 (RDS) 的 Windows 伺服器上，原先稱為終端機服務：
  
- 您必須具備包含 Office 365 ProPlus，例如 Office 365 企業版 E3 或企業 E5 的 Office 365 計劃。Office 365 企業版及 Office 365 企業進階版計劃不包含 Office 365 ProPlus。
    
- 您需要啟用[共用的電腦啟用](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。
    
如果您想要安裝 Office 365 ProPlus RDS 上從 Office 365 入口網站 * **以使用預設的安裝設定** *，請遵循下列步驟： 
  
1. 檢查您有哪些 Office 365 計劃。[了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. 如果需要，切換至不同的 Office 365 計劃。[了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. 如果使用任何其他 Office 365 計劃的 RDS 伺服器上已安裝 Office，請將它解除安裝。例如，依移至 [控制台]\>解除安裝程式。解除安裝使用[Microsoft 技術支援人員及復原小幫手]](https://aka.ms/SARA-OfficeUninstall-Alchemy)如果您正在執行發生問題。 
    
4. RDS 伺服器上，登入您的系統管理員帳戶和[安裝 Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)與 Office 365 入口網站。
    
5. 安裝 Office 之後，* **不開啟或登入** * 任何 Office 應用程式。 
    
6. RDS 伺服器上啟用共用的電腦啟用編輯登錄依照下列步驟：
    
1. 以滑鼠右鍵按一下您的螢幕左上角的 [Windows] 按鈕，並選取 [執行]。在 [開啟] 方塊中輸入**regedit**，，然後選取 [確定]。 
    
2. 選取 [是] 以允許登錄編輯程式中出現提示時變更您的裝置。
    
3. 在登錄編輯程式中，使用設定為 1 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 下新增**SharedComputerLicensing**的字串值。 
    
7. RDS 伺服器上 * **以使用者身分登入** * 並[確認已啟用共用的電腦啟用 Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。
    
如需必要條件、 安裝指示和指引自訂安裝使用 Office 部署工具的詳細資訊，請參閱[部署 Office 365 ProPlus 使用遠端桌面服務](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。
  
若要修正與共用的電腦啟動相關的錯誤，請參閱[共用的電腦啟用 Office 365 proplus 的疑難排解問題](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。
  

