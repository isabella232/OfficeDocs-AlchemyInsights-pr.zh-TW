---
title: Windows 10 中的 [電源] 或 [電池] 圖示遺失
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790539"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Windows 10 中的 [電源] 或 [電池] 圖示遺失

如果您的 Windows 10 裝置有電池 (例如，膝上型電腦或平板電腦，或透過 USB 連線到 UPS 的 PC)，通常會在工作列中的時鐘旁顯示電源/電池圖示，例如：

![電池圖示](media/battery-icon.png)

如果您沒有看到此圖示，則它可能為隱藏狀態：

1. 移至 **[[設定] > [個人化] > [工作列]](ms-settings:taskbar?activationSource=GetHelp)**。

2. 在 [通知區域] 中，按一下 **[選取要顯示在工作列上的圖示]**。

3. 然後在清單中找到 **[電源]** 項目，並將其設定切換為 **[開啟]**。

    ![在工作列中顯示電源圖示](media/power-icon-on.png)

**疑難排解**

如果您已依照上述指示，且 **[電源]** 切換開關呈現灰色或不可見，請在工作列上的 [搜尋] 方塊中輸入 **裝置管理員**，然後選取結果清單中的 **[裝置管理員]**。 在 **[電池]** 底下，以滑鼠右鍵按一下您裝置的電池，按一下 **[停用]**，然後按一下 **[是]**。 請稍候幾秒，然後以滑鼠右鍵按一下電池，然後按一下 **[啟用]**。 然後重新啟動您的裝置。

如果您依照上述指示操作，但電池圖示並未出現在工作列上，請在工作列上的 [搜尋] 方塊中輸入 **工作管理員**，然後在結果清單中按一下 **[工作管理員]**。 在 **[處理程序]** 索引標籤的 **[名稱]** 底下，以滑鼠右鍵按一下 **[檔案總管]**，然後按一下 **[重新啟動]**。
