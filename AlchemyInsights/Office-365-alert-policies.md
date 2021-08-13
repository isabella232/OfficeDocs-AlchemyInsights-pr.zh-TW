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
ms.openlocfilehash: 7bb5ec0efb7e29dc6a133d62491c7674c5a851a4fa422c647035aeaa0dbcd8d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918350"
---
# <a name="alert-policies"></a>警示原則

Microsoft 365 security & 規範中心提供[預設的警示原則](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)，可觸發具有 Office 365 企業版或 Office 365 美國政府 E1/G1、E3/G3 或 E5/G5 訂閱之組織的警示。 因此，系統管理員可能會收到 Office365Alerts@microsoft.com 使用主旨列（如「嚴重性警示： *警示原則的名稱*」）傳送的警示電子郵件通知。 當一般活動（例如使用者）觸發警示時，會傳送警示通知。

- 建立轉寄電子郵件的收件匣規則。
- 指派許可權給其信箱。
- 在 SharePoint 檔案共用中共用或刪除大量檔案。
- 建立 eDiscovery 搜尋並匯出搜尋結果。

若要複查並對警示採取動作：

1. 移至 [安全性 & 合規性中心](https://protection.office.com) 並登入。
2. 按一下 [**提醒**] [  >  **查看提醒**]。
3. 按一下警示以顯示彈出頁面，包含提醒的相關資訊。

您可以對警示採取動作，例如 [移除可疑的收件匣規則](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)。 或者，您只要在 [警示飛出] 頁面上按一下 [ **解析** ]，即可關閉警示。

如需設定及管理報警原則的詳細資訊，請參閱  [本文](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)。

**重要**：警示來自 Microsoft 的電子郵件通知，永遠不會要求您執行下列動作：

- 提供密碼
- 驗證帳戶的安全性詳細資料
- 重新驗證您的自我

如果您收到類似這封的電子郵件訊息，它並非 Microsoft 所傳送，應視為網路釣魚詐騙。 如果發生這種情況，請 [向 Microsoft 報告](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。