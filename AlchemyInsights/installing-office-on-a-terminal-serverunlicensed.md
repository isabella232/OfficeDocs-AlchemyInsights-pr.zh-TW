---
title: 終端機伺服器-未經授權上安裝 office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381720"
---
# <a name="installing-office-on-a-terminal-server"></a>終端機伺服器上安裝 Office

部署 Office 365 專業增強版使用遠端桌面服務 (RDS) 的 Windows 伺服器上，以前稱為終端機服務：
  
- 您必須擁有 Office 365 方案包含 Office 365 專業增強版，例如 Office 365 企業版 E3 或企業版 E5。 Office 365 商務版和 Office 365 商務進階版方案並未包含 Office 365 專業增強版。

- 您要啟用[共用的電腦啟用](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)。

如果您想要安裝 Office 365 專業增強版上 RDS 從 Office 365 入口網站，* **這麼做會使用預設安裝設定** *，請遵循下列步驟：
  
1. 請檢查您有哪些 Office 365 計劃。 [了解如何](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. 如果有需要時，切換至不同的 Office 365 計劃。 [了解如何](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. 如果使用任何其他 Office 365 計劃在 RDS 伺服器上已安裝 Office，請將它解除安裝。 例如，可以移至 [控制台]\>解除安裝程式。 解除安裝使用[Microsoft 的支援及修復小幫手](https://aka.ms/SARA-OfficeUninstall-Alchemy)，如果您正在執行發生問題。

4. 在 RDS 伺服器上，登入與您的系統管理員帳戶和[安裝 Office 365 專業增強版](https://portal.office.com/OLS/MySoftware.aspx)的 Office 365 入口網站。

5. 安裝 Office 之後，* **未開啟或登入** * 任何 Office 應用程式。

6. 在 RDS 伺服器上，啟用共用的電腦啟用編輯登錄遵循下列步驟：

1. 以滑鼠右鍵按一下您的螢幕左上角的 [Windows] 按鈕，選取 [執行]。 在 [開啟] 方塊中，輸入**regedit**，，然後選取 [確定]。

2. 選取 [是] 以允許登錄編輯程式出現提示時若要變更您的裝置。

3. 在登錄編輯程式中，使用設定為 1 下 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 新增**SharedComputerLicensing**的字串值。

7. 在 RDS 伺服器上，* **以使用者身分登入** *，並[確認 Office 365 專業增強版時啟用共用的電腦啟用](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。

如需必要條件、 安裝指示和指引自訂安裝使用 Office 部署工具的詳細資訊，請參閱[部署 Office 365 專業增強版使用遠端桌面服務](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)。
  
若要修正錯誤相關的共用的電腦啟用，請參閱[Office 365 專業增強版的共用的電腦啟用的疑難排解問題](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)。
  