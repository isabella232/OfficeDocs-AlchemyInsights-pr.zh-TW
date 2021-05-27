---
title: 受攻擊面縮小規則
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651478"
---
# <a name="attack-surface-reduction-rules"></a>受攻擊面縮小規則

排除檔案或資料夾可能會嚴重降低受攻擊面縮小規則所提供的保護。 允許執行規則所封鎖的檔案，而且不會記錄任何報告或事件。 排除會套用到允許排除的所有規則。

ASR 排除會使用與 Microsoft Defender 防毒軟體排除相同的語法。 如需詳細資料，請參閱[設定及驗證 Microsoft Defender 防毒軟體掃描的排除項目](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) (部分機器翻譯)。 若要避免問題，請檢閱[定義排除時應避免的常見錯誤](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus) (部分機器翻譯)。

並非所有 ASR 規則都支援排除。 若要驗證您的規則是否支援排除，請參閱[受攻擊面縮小規則](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)表格。

## <a name="attack-surface-reduction-rules"></a>受攻擊面縮小規則

您的組織受攻擊面包括攻擊者可能會危害組織裝置或網路的所有位置。 減少受攻擊面表示保護組織裝置和網路，減少攻擊者執行攻擊的方式。 在適用於端點的 Microsoft Defender 中設定受攻擊面縮小規則可以有所幫助。

如需詳細資訊，請參閱：

- [將 ASR 規則 GUID 對應到名稱](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR 規則需求：
    - [Windows 10 專業版，版本 1709 或更新版本](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 企業版，版本 1709 或更新版本](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server 版本 1803 (半年通道) 或更新版本](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>識別要套用的正確排除

1. 在 Microsoft-Windows-Windows Defender/Operational 記錄中尋找 eventID 1121 或 1122。

1. 評估區塊案例和內容，並確認此案例需要取消封鎖。

1. 讀取事件詳細資料中的 Path 值，這是定義排除的值。
    - 盡可能設定嚴格的排除。
    - 視需要套用萬用字元 (例如，取代 User 變數)。

1. 根據部署需求套用排除。 如需詳細資料，請參閱[自訂受攻擊面縮小規則](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction) (部分機器翻譯)。

## <a name="exclusion-is-not-honored"></a>未遵守排除

1. 判斷規則是否支援排除。 如需詳細資料，請參閱[受攻擊面縮小規則](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules) (部分機器翻譯)。

1. 檢閱套用的排除，並驗證事件資料是否包含錯字或解譯錯誤的萬用字元。 如需詳細資訊，請參閱[支援的排除類型](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types) (部分機器翻譯)

1. 如果規則的影響太高，請考慮將規則移到 (移回) 稽核模式，以執行進一步的驗證。 如需詳細資料，請參閱[測試適用於端點的 Microsoft Defender 功能在稽核模式中的運作方式](/microsoft-365/security/defender-endpoint/audit-windows-defender) (部分機器翻譯)。

1. 使用此命令收集支援資料以開啟支援案例：
    
   ** MDEClientAnalyzer.cmd -v**

    如需詳細資訊，請參閱[將電腦上線至適用於端點的 Microsoft Defender 的問題](issues-with-onboarding-machines.md)。
