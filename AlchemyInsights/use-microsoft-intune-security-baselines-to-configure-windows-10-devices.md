---
title: 使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641616"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>使用 Microsoft Intune 安全性基準來設定 Windows 10 裝置

Intune 安全性基準可協助保護使用者和裝置。 安全性基準是 Windows 設定的預先設定群組，用來套用相關安全小組建議的已知設定群組和預設值。 透過在 Intune 中建立安全性基準設定檔，您可以建立由多個裝置群組原則檔組成的範本。

當您將安全性基準部署至使用者或裝置群組時，這些設定會套用於在 Windows 10 或更新版本上執行的裝置。 例如，Microsoft 行動裝置管理 (MDM) 安全性基準會自動 (1) 啟用抽取式磁碟機的 BitLocker、(2) 需要密碼才能解除鎖定裝置，以及 (3) 停用基本驗證。 當預設值不適用於您的環境時，您可以自訂基準以套用所需的設定。

安全性基準也可協助在 Microsoft 365 中建立端對端安全工作流程。 以下是此功能的一些益處：
- 安全性基準包含影響安全性之設定的最佳作法和建議。 由於 Intune 與建立群組原則基準的 Windows 安全性小組合作，因此這些建議是以可靠的指引和廣泛的經驗為基礎。
- 如果您第一次使用 Intune 且不確定從何處開始，則安全性基準將可協助快速建立及部署安全的設定檔。
- 如果您目前正使用群組原則，則搭配安全性基準移入 Intune 來用於管理目的會更容易，因為這些安全性基準內建在 Intune 中，並包含用於管理的最先進功能。

如需詳細資訊，請參閱 [Windows 安全性基準](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines)以及[行動裝置管理](https://docs.microsoft.com/windows/client-management/mdm/)。