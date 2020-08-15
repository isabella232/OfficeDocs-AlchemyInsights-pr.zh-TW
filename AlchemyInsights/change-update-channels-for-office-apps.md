---
title: 變更 Office 應用程式的更新通道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 3e1042a38d2289b9ef2396e8300d32f20ddaa703
ms.sourcegitcommit: b5e5f560bf6ef92b4475bd3d91b7df38b5a4b036
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/14/2020
ms.locfileid: "46739818"
---
# <a name="change-update-channels-for-office-apps"></a>變更 Office 應用程式的更新通道

對於新的 Office 安裝，請使用 Office 軟體下載設定選取所需的更新頻道，然後安裝 (或重新安裝) Office 應用程式。   如需詳細資訊， 請參閱 [管理 Office 365 中的軟體下載設定](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365)。 

**附註** 使用 Office 軟體下載設定選取的更新通道適用于使用 O365 入口網站執行新安裝的所有使用者。 如需更多資訊，請參閱 [在 PC 或 Mac 上下載並安裝或重新安裝 Microsoft 365 或 Office 2019](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658)。   

對於現有的 Office 安裝，請使用 Office 部署工具 (ODT) 切換到其他更新通道：  

1. 從 [Microsoft 下載中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下載最新版的 Office 部署工具 (setup.exe)。
2. 識別要切換到的通道名稱。 如需詳細資訊，請參閱 [Office 部署工具的設定選項](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element)。
3. 建立指定適當的通道名稱的組態 XML 檔案，例如 update.xml。  

`<Configuration>`<br>
`<Updates Channel="Monthly"/>`<br>
`</Configuration>`<br>

4. 在已提升權限的命令提示字元下，切換至 setup.exe 所在的資料夾，接著執行下列命令：  
    a. setup.exe /configure update.xml
5. 啟動 Office 應用程式 (例如 Excel)，然後選取 **[檔案]** > **帳戶**。 在 [產品資訊] 區段，選取 **[更新選項]** > ** [立即更新]**。

如需更多資訊，請參閱 [如何切換現有 Office 應用程式的更新頻道](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel)。 

要切換選定使用者群組的更新通道或使用組態管理員 (SCCM)，請使用 GPO 設定更新通道設定。 如需詳細資訊，請參閱 [Microsoft 365 Apps 更新通道的概觀](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy)。 如需詳細資訊，請參閱 [如何管理 Office 365 專業增強版 (IT 專業人員)](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) 和 [使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 Apps 的更新](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)。