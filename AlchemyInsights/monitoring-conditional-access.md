---
title: 監視條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366419"
---
# <a name="monitoring-conditional-access-for-exchange"></a>監視 Exchange 的條件式存取

以條件式存取為目標的使用者，如果不符合您組織的存取需求，將會收到通知電子郵件。 若要解決此問題，我們建議下列一或多個解決方案：

- 若要對裝置進行註冊，請建議使用者移至公司入口網站，並確認該應用程式出現在公司入口網站。 如果不是，則使用者應該註冊裝置。
- 在 Azure 入口網站中，移至 Intune > 裝置規範。 在 [監視器] 底下按一下 [裝置符合性]。 查看您的裝置符合性報告，以確認使用者的裝置已標示為相容。
- 在 Azure 入口網站中，移至 Intune > 裝置規範。 在 [管理] 下，按一下 [原則]。 在 [規範原則] 清單中，確認已將設定檔指派給您的使用者裝置。 若未指派設定檔，則 Intune 將無法確認裝置的符合性狀態。
- 編輯使用者的條件式存取指派。

1. 在 Azure 入口網站中，移至**Intune**  >  **條件式存取**  >  **原則**。
2. 從清單中選取原則。
3. 按一下 [使用者和群組]。
4. 若要以某人為目標設定特定原則，請將其新增至 [包含] 清單。 若要確保從原則中省略了某個人員，請將其新增至 [排除] 清單。

有用的連結：

[裝置合規性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[疑難排解 CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[疑難排解原則](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[監控 Intune 裝置合規性](https://docs.microsoft.com/intune/compliance-policy-monitor)

附注：這些步驟僅有助於疑難排解 Azure Active Directory 功能條件式存取。 您也可以隔離透過 Exchange 原則封鎖它的電子郵件存取的裝置。 您可以在 [這裡](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)找到 Exchange 裝置管理的詳細資訊。
