---
title: 反垃圾郵件-5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932160"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>修正錯誤碼為5.7.23 的電子郵件傳遞問題

在 web 上公開提供的 SPF 或 DNS 記錄檢查，確認您網域的 SPF DNS 記錄。

確認輸出郵件未被 Microsoft 識別為垃圾郵件，並透過 [高風險傳遞集](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)區路由傳送。 高風險傳遞集區中的郵件不會通過 SPF 檢查，因此目的地電子郵件組織不會接受此項功能。

如果問題持續發生，您可能需要與您嘗試傳送電子郵件的郵件主機系統管理員聯繫。 請記下退回郵件中提供的詳細外部錯誤。 Microsoft 支援部門可能無法進一步協助。
