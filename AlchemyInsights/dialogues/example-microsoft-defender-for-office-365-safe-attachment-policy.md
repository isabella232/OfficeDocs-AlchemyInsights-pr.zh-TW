---
title: Microsoft Defender for Office 365 安全附件原則範例
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530078"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Microsoft Defender for Office 365 安全附件原則範例

這些設定可讓未設定 *延遲* 的原則立即傳遞郵件，然後在掃描後將附件：

- **名稱**：無延遲
- **描述**：在掃描之後立即傳遞郵件並將附件。
- **回應**：選取 **動態傳遞** 選項。 如需詳細資訊，請參閱 [在安全附件原則中的動態傳遞](https://go.microsoft.com/fwlink/?linkid=2092328)。
- 重新 **導向附件** 區段：選取可 **啟用重新導向** 的選項，然後輸入您的 Microsoft 365 全域系統管理員、安全性管理員或將調查惡意附件的安全性分析員的電子郵件地址。
- **適用** 于區段：選取 **[收件者網域是**]，然後選取您的網域。 選取 [ **新增**]，然後選取 **[確定]**。 完成後，請選取 [ **儲存**]。

若要深入瞭解，請參閱 [Microsoft Defender For Office 365 中的安全附件](https://go.microsoft.com/fwlink/?linkid=2092213)。
