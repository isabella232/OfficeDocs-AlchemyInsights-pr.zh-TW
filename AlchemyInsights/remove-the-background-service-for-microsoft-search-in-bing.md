---
title: 移除 Bing 專用 Microsoft 搜尋的背景服務
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753392"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>移除 Bing 專用 Microsoft 搜尋的背景服務

若要移除 Bing 專用 Microsoft 搜尋的背景服務，您可以嘗試下列補救方法：

1. 若要還原為原始搜尋引擎設定，請執行下列操作：

    a. 將 [使用 Bing 做為預設搜尋引擎]**[ 開關切換為 [關閉]](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**。

    b. [前往 Microsoft 365 系統管理中心](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)並清除會影響組織中所有使用者的設定。

2. 若要從個別裝置移除背景服務，請執行下列工作：

    a. 選擇 **[控制台] > [程式集] > [程式和功能]**。

    b. 在目前安裝程式的清單中，以滑鼠右鍵按一下 **[Bing 專用 Microsoft 搜尋]**，然後再按一下 **[解除安裝]**。

3. 若要從組織中多個裝置移除背景服務，請以系統管理員身分登入，然後執行指令碼中的下列命令： 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
