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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500823"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>修正 DKIM 記錄格式設定的常見問題

大部分 DKIM 的設定問題與不正確的 DNS 記錄有關。

若要修正 DKIM 的設定問題，請確認 DKIM CNAME 記錄 (**不** 是 TXT 記錄) 的格式是否正確。 如需詳細資訊，請參閱 [在 Office 365 中手動設定 DKIM 所需執行](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)的動作。

如果您一般都需要 DNS 記錄的協助，請參閱 [在任何 dns 主機服務提供者處建立 dns 記錄，以進行 Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。

> [!NOTE]
> 在您的網域的 DNS 主機服務上建立或更新 DKIM DNS 記錄之後，您必須等待 DNS 記錄傳播。
