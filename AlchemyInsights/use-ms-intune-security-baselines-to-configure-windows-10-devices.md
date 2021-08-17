---
title: 使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104335"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置

Intune 安全性基準可協助保護使用者和裝置。 安全性基準是 Windows 設定的預先設定群組，用來套用相關安全小組建議的已知設定群組和預設值。 透過在 Intune 中建立安全性基準設定檔，您可以建立由多個裝置群組原則檔組成的範本。

當您將安全性基準部署至使用者或裝置群組時，設定會套用至在 Windows 10 或更新版本上執行的裝置。 例如，MDM 安全性基準會自動 (1) 啟用抽取式磁碟磁碟機 BitLocker， (2) 需要密碼才能解除裝置鎖定，而 (3) 會停用基本驗證。 當預設值不適用於您的環境時，請自訂基準來套用您所需的設定。

安全性基準也可協助在 Microsoft 365 中建立端對端安全工作流程。 以下是一些優點：

- 安全性基準包含影響安全性之設定的最佳作法和建議。 由於 Intune 與建立群組原則基準的 Windows 安全性小組合作，因此這些建議是以可靠的指引和廣泛的經驗為基礎。
- 如果您第一次使用 Intune 且不確定從何處開始，則安全性基準將可協助快速建立及部署安全的設定檔。
- 如果您目前使用群組原則，將安全性基準遷移到 Intune 以進行管理，因為它們已內置於 Intune 中，且包含用於管理的前沿功能。

若要深入瞭解，請參閱[Windows 安全性基準](https://go.microsoft.com/fwlink/?linkid=2141503)及行動[裝置管理](https://go.microsoft.com/fwlink/?linkid=2141701)。