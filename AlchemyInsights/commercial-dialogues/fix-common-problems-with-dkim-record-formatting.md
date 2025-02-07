---
title: 修正 DKIM 記錄格式設定的常見問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323981"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>修正 DKIM 記錄格式設定的常見問題

大部分 DKIM 的設定問題與不正確的 DNS 記錄有關。

若要修正 DKIM 的設定問題，請確認 DKIM CNAME 記錄 (**不** 是 TXT 記錄) 的格式是否正確。 如需詳細資訊，請參閱[在 Office 365 中手動設定 DKIM 時所需執行](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)的動作。

如果您一般都需要 DNS 記錄的協助，請參閱[在 Office 365 的任何 DNS 主機服務提供者中建立 dns 記錄](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。

**附注**：在您的網域的 DNS 主機服務上建立或更新 DKIM DNS 記錄之後，您將需要等候 DNS 記錄傳播。
