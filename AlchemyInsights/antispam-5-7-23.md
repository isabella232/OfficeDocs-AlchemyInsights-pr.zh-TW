---
title: 反垃圾郵件-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682056"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>修正電子郵件傳遞問題的錯誤碼 5.7.23

確認在 web 上公開提供 SPF 或 DNS 記錄檢查您網域的 SPF DNS 記錄。

確認輸出郵件未由 Office 365 識別為垃圾郵件，並透過[高風險傳遞集區](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)路由傳送。 高風險傳遞集區中的郵件將不會通過 SPF 檢查，並因此將不會接受的目的地電子郵件組織。

如果問題仍然存在，您可能需要連絡您嘗試傳送電子郵件的郵件主機的系統管理員。 請記下詳細的外部錯誤用於退回的郵件。  Office 365 支援人員可能無法進一步協助。