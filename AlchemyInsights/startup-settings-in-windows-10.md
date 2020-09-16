---
title: Windows 10 中的啟動設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751126"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10 中的啟動設定

**變更啟動時自動執行的應用程式**

1. 移至 [ [設定] > 應用程式 > 啟動](ms-settings:startupapps?activationSource=GetHelp)。

2. 請確定開啟時您想要 **執行的任何**應用程式已開啟。

**新增應用程式，以在啟動時自動執行**

1. 按一下或點擊 [ **開始** ]，尋找您想要在啟動時執行的應用程式。

2. 以滑鼠右鍵按一下應用程式，按一下 [ **其他**]，然後按一下 [ **開啟檔案位置**]。 這會開啟儲存應用程式快捷方式的位置。 如果開啟的檔案位置沒有任何選項，則表示應用程式無法在啟動時執行。

3. 在檔案位置開啟時，按 **Windows 徽標鍵 + R**，輸入命令介面 **： startup**，然後按一下 **[確定]**。 這會開啟 [啟動] 資料夾。

4. 從檔案位置複製並貼上應用程式的快捷方式至 [啟動] 資料夾。

**Advanced startup options (包括安全模式、UEFI 設定，以及從另一個裝置引導) **

1. 儲存您的工作並關閉任何開啟的檔，因為這些步驟將會重新開機您的電腦。

2. 移至 [ [設定] > 更新 & Security > Recovery](ms-settings:recovery?activationSource=GetHelp)。

3. 在 [ **Advanced startup**] 底下，按一下 [ **立即重新開機**]。 

4. 在您的電腦重新開機至 [選擇選項] 畫面之後：

    - 若要從 USB 磁片磁碟機等設備進行引導，請按一下 [ **使用裝置**]。

    - 若要輸入 UEFI 設定 (有時稱為 BIOS 設定) ，請按一下 [ **疑難排解] > 高級選項 > UEFI 固件設定**。 

    - 若要輸入安全模式或變更 [advanced startup] 設定，請按一下 [ **疑難排解 > 高級選項] > 啟動設定**]，然後按一下 [ **重新開機**]。 您可能會要求您輸入 [BitLocker 復原金鑰](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)。 重新開機電腦之後，按一下您要使用的啟動設定。