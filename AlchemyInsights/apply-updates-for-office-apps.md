---
title: 套用 Office 應用程式的更新
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
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969376"
---
# <a name="apply-updates-for-office-apps"></a>套用 Office 應用程式的更新

根據預設，從網際網路免費自動下載並在背景中套用 Office 應用程式的更新，不需要任何使用者介入。 如果在應用更新時遇到問題，請手動運行更新， 請參閱 [安裝 Office 更新](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)。 如需詳細資訊，請參閱[Office 安裝問題的疑難排解](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)。

若要為您的使用者管理 Office 更新，請考慮下列選項：

- 根據所需的更新頻率為您的組織選擇正確的 Office 更新通道。 若要了解做法，請參閱 [Microsoft 365 Apps 更新通道的概觀](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)。

- 决定從網際網路還是內部部署自動套用更新。 若要了解做法，請參閱 [選擇如何管理 Microsoft 365 Apps 的更新](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)。

- 查看 Office 更新設定，以控制將更新套用於使用者電腦的方式:

    - [設定 Microsoft 365 Apps 的更新設定](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)。
    - [定義安裝 Office 之後如何更新](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)。

當您將 Office app 部署到多個使用者時，請使用 Office 自訂工具來建置部署設定檔，並使用 Office 部署工具來設定 Office 更新。 如需詳細資訊，請參閱 [Office 自訂工具概觀](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) 和 [Office 部署工具](https://go.microsoft.com/fwlink/p/?LinkID=626065)。

- 如需如何設定使用者群組以部署 Office 更新的範例，請參閱 [從本機來源部署 Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)。
-   考慮使用 ForceAppShutdown 設定，以防 Office 更新由於打開的 Office 應用程式而無法套用於少數使用者。 有關詳細資訊，請參閱 [FORCEAPPSHUTDOWN 屬性 (Property 元素的一部分)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element)。 

**另請參閱**

[Microsoft 365 Apps 更新程序概觀](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)。  
[Microsoft 365 Apps 更新的版本資訊](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)。  
[使用 Microsoft Endpoint Configuration Manager 管理 Microsoft 365 Apps 的更新](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)。  
