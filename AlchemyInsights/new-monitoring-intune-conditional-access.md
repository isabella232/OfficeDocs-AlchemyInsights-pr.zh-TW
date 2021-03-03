---
title: 監視 Intune 條件式存取
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417110"
---
# <a name="monitor-intune-conditional-access"></a>監視 Intune 條件式存取

以條件式存取為目標的使用者，如果不符合您組織的存取需求，將會收到通知電子郵件。 若要解決此問題，我們建議下列一或多個解決方案：

1. 若要對裝置進行註冊，請建議使用者移至公司入口網站，並確認該應用程式出現在公司入口網站。 如果不是，則使用者必須註冊裝置。
1. 在 Azure 入口網站中，移至 **Intune**  >  **裝置規範**。 
1. 若要查看您的裝置符合性報告，以確認使用者的裝置標示為相容，請按一下 [ **監視器**] 底下的 [ **裝置符合性**]。
1. 在 Azure 入口網站中，移至 **Intune**  >  **裝置規範**。 在 [管理] 下 **，** 按一下 [ **原則**]。 在 [規範原則] 清單中，確認已將設定檔指派給您的使用者裝置。 若未指派設定檔，則 Intune 將無法確認裝置的符合性狀態。
1. 編輯使用者的條件式存取指派。
1. 在 Azure 入口網站中，流覽至 [ **Intune**  >  **條件式存取**  >  **原則**]，從清單中選取原則，然後按一下 [**使用者和群組**]。
1. 若要以某人為目標設定特定原則，請將其新增至 [ **包含] 清單**。 若要確保從原則中省略了某個人員，請將其新增至 [ **排除] 清單**。

**有用的連結：**

- [裝置合規性概述](https://docs.microsoft.com/intune/device-compliance-get-started)
- [疑難排解 CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [疑難排解原則](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [監控 Intune 裝置合規性](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> 這些步驟只有助于疑難排解 Azure Active Directory 功能條件式存取。 您也可以隔離透過 Exchange 原則封鎖它的電子郵件存取的裝置。 您可以在 [**這裡**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))找到 Exchange 裝置管理的詳細資訊。
