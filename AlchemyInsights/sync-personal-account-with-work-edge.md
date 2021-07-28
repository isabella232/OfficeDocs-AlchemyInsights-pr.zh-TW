---
title: 讓使用者在 Microsoft Edge 中將個人帳戶與公司帳戶同步
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: 4c246fcc9ef0e3a79c3e68be491e3e7f5c6edb0b
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603234"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>讓使用者在 Microsoft Edge 中將個人帳戶與公司帳戶同步

請確定您符合以下準則：

- Azure Active Directory 系統管理中心已啟用 [企業狀態漫遊]，其需要訂閱 Azure Active Directory Premium 或 Enterprise Mobility + Security (EMS)。 如需詳細資訊，請參閱[在 Azure Active Directory 中啟用企業狀態漫遊](/azure/active-directory/devices/enterprise-state-roaming-enable) (部分機器翻譯)。
- 符合下列其中之一或兩個準則：
    - 您的租用戶已啟用 Azure 資訊保護服務。 如需詳細資料，請參閱[從 Microsoft 365 系統管理中心網站啟動 Azure Rights Management 保護](/azure/information-protection/activate-office365) (部分機器翻譯)。
    - 已針對所有使用者或租用戶啟用 Azure Active Directory 企業狀態漫遊 (ESR) 功能。 如需詳細資訊，請參閱[什麼是企業狀態漫遊？](/azure/active-directory/devices/enterprise-state-roaming-overview) (部分機器翻譯)。

如果 AIP 和 ESR 都停用，會有錯誤訊息通知使用者其帳戶無法使用同步處理。
