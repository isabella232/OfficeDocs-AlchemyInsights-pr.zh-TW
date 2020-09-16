---
title: 控制 Office 應用程式自動更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747767"
---
# <a name="control-automatic-updates-for-office-apps"></a>控制 Office 應用程式自動更新

根據預設，從網際網路自動下載並在背景中套用 Office 應用程式的更新，不需要任何使用者介入。 不過，系統管理員可以使用 Office [更新] 設定來控制應用更新的方式。 [更新] 設定允許系統管理員啟用或停用自動更新、顯示或隱藏 Office 中的 **[立即更新]** 按鈕、設定更新期限等。 如需詳細資訊，請參閱：

- [設定 Office 更新設定](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [未啟用 Office 自動更新](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [定義安裝 Office 之後如何更新](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

若要查看套用至用戶端電腦的現有更新設定，請遵循下列步驟：

1. 若要開啟 [登錄編輯程式]，請移至 **[開始]** > **[執行]** > **regedit**。
2. 切換到下列位置，並查看 Office [更新] 設定：  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**附註** 如果已設定 OfficeMgmtCOM 機碼，可能會在 **Office** > **帳戶** > ** Office 更新**中看到「由系統管理員管理更新」的訊息。 如需更多資訊，請參閱[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 Apps 的更新](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)。  