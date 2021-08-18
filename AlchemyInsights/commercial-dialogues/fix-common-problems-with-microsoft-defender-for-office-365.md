---
title: 修正 Microsoft Defender Office 365 的常見問題
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330051"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>修正 Microsoft Defender Office 365 的常見問題

以下是 Microsoft Defender Office 365 的常見問題的解決方案：

- **郵件延遲**：

  電子郵件傳遞的延遲可能會因保管庫電子郵件的附件掃描而造成。 如需詳細資訊，請參閱[保管庫附件原則設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)。

- **報告 false 的肯定或否定的結果**：

  如需詳細資訊，請參閱[回報訊息和檔案至 Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)。

- **啟用保管庫連結保護**：

  1. 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com/> ，移至 **電子郵件 &** 共同作業 \> **原則 & 規則** \> **威脅原則** \> **保管庫** 的 **原則]** 區段中的連結。

     若要直接移至 [**保管庫連結**] 頁面，請使用 <https://security.microsoft.com/safelinksv2> 。

  2. 在 [**保管庫連結**] 頁面上，按一下原則的名稱以選取原則。
  3. 在出現的 [詳細資料] 浮出控制項中，執行下列其中一個步驟：
     - 若要新增原則，請選取 [ **+ 建立**]。 嚮導將啟動以協助您定義原則設定。
     - 若要編輯現有的原則，請按一下原則的名稱以選取原則。 在出現的 [詳細資料] 快顯視窗中，選取 [**保護設定**] 區段中的 [**編輯**]。
  4. 在 [ **保護設定** ] 頁面上，設定下列設定：
     - 開啟 **[選取郵件中未知可能惡意 URLs 的動作**]。
     - 選取 **[套用安全連結] 至組織內所傳送的郵件**。

  如需詳細資訊，請參閱[在 Microsoft Defender for Office 365 中設定保管庫連結原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)。
