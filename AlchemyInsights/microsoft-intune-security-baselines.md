---
title: 使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 0a89b121f2f425b0a81fa250650f108e9af48c9da39dfc8a62b07541d3a6c3dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098053"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置

Intune 安全性基準可協助保護使用者和裝置。 安全性基準 Windows 設定預先設定的群組，用來套用已知的設定群組和相關的安全性小組建議的預設值。 透過在 Intune 中建立安全性基準設定檔，您可以建立由多個裝置群組原則檔組成的範本。

當您將安全性基準部署至使用者或裝置群組時，設定會套用至在 Windows 10 或更新版本上執行的裝置。 例如，Microsoft 行動裝置管理 (MDM) 安全性基準會自動啟用抽取式磁碟磁碟機 BitLocker、需要密碼以解除鎖定裝置，以及停用基本驗證。 當預設值不適用於您的環境時，您可以自訂基準以套用所需的設定。

安全性基準也可協助在 Microsoft 365 中建立端對端安全工作流程。 安全性基準包含影響安全性之設定的最佳作法和建議。 Intune 合作夥伴使用 Windows 安全小組為群組原則建立基準，所以這些建議是以堅實的指導和廣泛的經驗為基礎。

如果您是最新的 Intune，且不確定開始位置，安全性基準會協助您快速建立及部署安全的設定檔。 如果您目前使用群組原則，由於安全性基準已內置於 Intune 中，所以針對管理目的遷移至 Intune 會更容易，並包含切削 edge 的管理功能。

若要深入瞭解，請參閱[Windows 安全性基準](/windows/security/threat-protection/windows-security-baselines)及行動[裝置管理](/windows/client-management/mdm/)。

