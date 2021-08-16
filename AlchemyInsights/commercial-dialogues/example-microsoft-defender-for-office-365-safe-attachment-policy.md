---
title: Office 365 保管庫附件原則的 Microsoft Defender 範例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988286"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Office 365 保管庫附件原則的 Microsoft Defender 範例

這些設定可讓未設定 *延遲* 的原則立即傳遞郵件，然後在掃描後將附件：

- **名稱**：無延遲
- **描述**：在掃描之後立即傳遞郵件並將附件。
- **回應**：選取 **動態傳遞** 選項。 如需詳細資訊，請參閱[保管庫附件原則中的動態傳遞](https://go.microsoft.com/fwlink/?linkid=2092328)。
- 重新 **導向附件** 區段：選取可 **啟用重新導向** 的選項，然後輸入您 Microsoft 365 全域系統管理員、安全性管理員或將調查惡意附件的安全性分析員的電子郵件地址。
- **適用** 于區段：選取 **[收件者網域是**]，然後選取您的網域。 選取 [ **新增**]，然後選取 **[確定]**。 完成後，請選取 [ **儲存**]。

若要深入瞭解，請參閱[保管庫 Office 365 的 Microsoft Defender 附件](https://go.microsoft.com/fwlink/?linkid=2092213)。
