---
title: 1385-Office-365-警示原則
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312678"
---
# <a name="alert-policies"></a>警示原則

Microsoft 365 包含[預設的警示原則](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)，可觸發具有 Microsoft 365 企業版或 Microsoft 365 美國政府 E1/G1、E3/G3 或 E5/G5 訂閱的組織警示。 因此，系統管理員可能會收到 Office365Alerts@microsoft.com 使用主旨列（如「嚴重性警示： *警示原則的名稱*」）傳送的警示電子郵件通知。 當一般活動（例如使用者）觸發警示時，會傳送警示通知。

- 建立轉寄電子郵件的收件匣規則。
- 指派許可權給其信箱。
- 在 SharePoint 檔案共用中共用或刪除大量檔案。
- 建立 eDiscovery 搜尋並匯出搜尋結果。

若要複查並對警示採取動作：

1. 執行下列其中一個步驟：
   - 在 [Microsoft 365 合規性中心于] 中 <https://compliance.microsoft.com> ，移至 **警示**。 或者，若要直接移至 [ **提醒** ] 頁面，請使用 <https://compliance.microsoft.com/compliancealerts> 。
   - 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**事件] & 警示** \> **警示**。 或者，若要直接移至 [ **提醒** ] 頁面，請使用 <https://security.microsoft.com/alerts> 。
2. 按一下警示以顯示彈出頁面，包含提醒的相關資訊。

您可以對警示採取動作，例如 [移除可疑的收件匣規則](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)。 或者，您只要在 [警示飛出] 頁面上按一下 [ **解析** ]，即可關閉警示。

如需設定及管理報警原則的詳細資訊，請參閱  [本文](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)。

**重要**：警示來自 Microsoft 的電子郵件通知，永遠不會要求您執行下列動作：

- 提供密碼
- 驗證帳戶的安全性詳細資料
- 重新驗證您的自我

如果您收到具有這類要求的電子郵件，它不是由 Microsoft 傳送，也應視為網路釣魚詐騙。 如果您收到具有這類要求的郵件，請將 [郵件報告給 Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)。
