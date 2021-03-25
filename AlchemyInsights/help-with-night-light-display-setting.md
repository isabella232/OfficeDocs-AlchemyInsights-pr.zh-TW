---
title: 夜間光線顯示設定說明
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123042"
---
# <a name="help-with-the-night-light-display-setting"></a>夜間光線顯示設定說明

若要深入了解夜間顯示設定，請參閱 [在 Windows 10 中設定顯示器於夜間使用](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)。

如果夜間光線選項在 [設定] 中顯示為灰色，請檢查您的顯示器驅動程式： 

1. 按一下工作列上的搜尋方塊，然後輸入 **[裝置管理員]**，然後在搜尋結果中選取 **[裝置管理員]**。
1. 展開 **[顯示卡]**。 

很抱歉，如果您的裝置使用 DisplayLink 驅動程式或基本顯示器驅動程式，夜間光線功能將不可用。

夜間光線功能會使用最新的圖形技術，因此您可能需要更新顯示器驅動程式：  

- 若要檢查更新，請前往 **[開始]** > **[設定]** > **[更新與安全性]** > **[Windows Update]** > **[檢查更新]**。  

或

- 請瀏覽硬體製造商的支援網站，以手動下載並安裝最新的顯示器驅動程式。

## <a name="reset-night-light-in-the-registry"></a>重設登錄中的夜間光線

如果更新顯示器驅動程式未起作用，您可能需要在登錄中重設夜間光線。  

**注意：** 只建議進階使用者使用這個疑難排解步驟。 如果未能正確修改登錄，可能會發生嚴重的問題。 若要增添一層防護，請先備份登錄再進行修改。如此一來，如果發生問題，您便能加以還原。

1. 在搜尋方塊中，輸入 **regedit**，然後在搜尋結果中選取 **[登錄編輯程式]**。

1. 移至下列登錄機碼： 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. 匯出然後刪除下列子機碼：$$windows.data.bluelightreduction.bluelightreductionstate

1. 匯出然後刪除下列子機碼：$$windows.data.bluelightreduction.settings

1. 重新啟動 Windows，並驗證夜間光線選項是否可用。


