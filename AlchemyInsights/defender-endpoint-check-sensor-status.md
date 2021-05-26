---
title: Defender 端點檢查感應器狀態
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627233"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender 端點檢查感應器狀態

**有感應器問題的裝置** 磚位於安全性作業儀表板上。 此磚提供有關個別裝置提供感應器資料和與適用於端點的 Defender 服務通訊的能力之資訊。 它報告需要注意的裝置數量，並協助您識別有問題的裝置並採取措施修正已知問題。

磚上的兩個狀態指示器提供有關未正確向服務報告的裝置數量之資訊：

- **設定錯誤** 可能部分向適用於端點的 Defender 服務報告感應器資料並且可能存在需要修正的設定錯誤之裝置。
- **閒置中** 過去一個月內超過 7 天未向適用於端點的 Defender 服務報告的裝置。

按一下任何群組都會將您導向至裝置清單，並根據您的選擇進行篩選。 在裝置清單中，可以按以下狀態篩選健康情況狀態清單：

- **作用中** 不斷向適用於端點的 Defender 服務報告的裝置。
- **設定錯誤** 可能部分向適用於端點的 Defender 服務報告感應器資料但存在需要修正的設定錯誤之裝置。 設定錯誤的裝置可能存在以下一個或多個問題：

    - 無感應器資料 - 裝置已停止傳送感應器資料。 裝置可以觸發有限的警示。
    - 通訊受損 - 與裝置通訊的能力受損。 傳送檔案進行深入分析、封鎖檔案、將裝置與網路隔離以及其他需要與裝置通訊的動作可能無法運行。
- **閒置中** 已停止向適用於端點的 Defender 服務報告的裝置。

您可以使用匯出功能以 CSV 格式下載整個清單。

如需詳細資訊，請參閱[檢查適用於端點的 Microsoft Defender 中的感應器健全狀態](/microsoft-365/security/defender-endpoint/check-sensor-status)。

如需導致裝置處於裝置狀態或設定錯誤的原因之詳細資訊，請參閱 [修正適用於端點的 Microsoft Defender 中的不良感應器](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)。
