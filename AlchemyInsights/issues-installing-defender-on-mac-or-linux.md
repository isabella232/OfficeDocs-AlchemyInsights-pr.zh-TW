---
title: 在 Mac 或 Linux 上安裝 Microsoft Defender 的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768385"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>在 Mac 或 Linux 上安裝 Microsoft Defender 的問題

**Mac**

- 安裝適用於 Mac 的 Microsoft Defender ATP 之前，請先確保已符合系統需求。 如需詳細資訊，請參閱[如何安裝適用於 Mac 的 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)。  
- 檢閱此檔案中的資訊："/Library/Logs/Microsoft/mdatp/install.log"。

**Linux**

- 安裝適用於 Linux 的 Microsoft Defender ATP 之前，請先確保已符合系統需求。 如需詳細資訊，請參閱[如何安裝適用於 Linux 的 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。 
- 若要確認 MDATP 服務執行中，請參閱[安裝失敗](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)。  
    若要疑難排解並解決服務未執行的問題，請參閱 [mdatp 服務未執行時的疑難排解步驟](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)。
- 如需檢查用戶端設定 (其會驗證產品的健康情況) 的步驟，以及若要對 EICAR 文字檔案執行偵測測試，請參閱[用戶端設定](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)。  

    **附註** 如需即時監視活動支援的檔案系統清單，請參閱[適用於 Linux 的 Microsoft Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。