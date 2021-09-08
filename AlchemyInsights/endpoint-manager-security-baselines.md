---
title: 端點管理員 - 安全性基準
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923545"
---
# <a name="endpoint-manager---security-baselines"></a>端點管理員 - 安全性基準

安全性基準是預先設定的 Windows 設定群組，可協助您套用相關安全小組建議的安全性設定。 您可以自訂這些基準，以只提供所需的設定和值。 如需安全性基準的詳細資訊，請參閱[在 Intune 中使用安全性基準來設定 Windows 10 裝置](https://docs.microsoft.com/mem/intune/protect/security-baselines)。

這些產品目前有基準：

- Windows MDM 安全性設定
- 適用於端點的 Microsoft Defender 安全性
- Microsoft Edge

每個基準會定期更新，並且以增量版本形式發行。 每個版本會新增或移除舊版的設定，以確保該基準符合目前的指導方針。 端點安全性中的安全性基準主控台透過讓不同版本的變更可顯示，以比較不同的版本。

如需如何最有效地變更所部署基準版本的指引，請參閱[在 Microsoft Intune 中管理安全性基準設定檔](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)。

部署安全性基準之後，您可以監視部署狀態，並依據裝置檢查設定。

由於安全性基準包含許多設定，因此必須檢閱設定變更並執行測試，以確保所有設定都適用於您的裝置和業務需求。

**注意：** 從初始部署到裝置可能需要最多 24 小時才能顯示比較基準的報告資料，且可能需要 6 小時，才能取得進一步的更新。 

基準設定不適用最常見的原因是在已在不同的設定檔中使用相同的設定。 您可以在安全性基準設定檔的 [裝置狀態] 節點內選取裝置，以調查特定裝置的狀況。 如需詳細資料，請參閱[解決安全性基準的衝突](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)。