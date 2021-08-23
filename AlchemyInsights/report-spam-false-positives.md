---
title: 您是否要將垃圾郵件誤報報告給 Microsoft？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396606"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>您是否將合法的郵件標示為垃圾郵件？

當垃圾郵件會在 [垃圾郵件] 資料夾或隔離區中結束時，會令人感到沮喪。 請考慮下列最常見的誤報原因：

**租使用者覆寫 (最常見)** 這完全是您要修正的控制項內。

在 Microsoft 365 Defender 上提交郵件以供分析影響的原則和規則;在幾分鐘內提供重新掃描的詳細資料。
查看或修改原則或規則（如果適用）。 

**End-User 會覆寫 (通用)** 這完全是您要修正的控制項內。 

在 Microsoft 365 Defender 上提交郵件以供分析影響的原則和規則;在幾分鐘內提供重新掃描的詳細資料。 

如果郵件因從使用者的封鎖寄件者清單中的位址傳送而遭到封鎖，則標頭會包含垃圾郵件篩選判定為 "SFV:BLK"。

**寄件者的電子郵件驗證** 這部分在您的控制項中以進行修正。

提交郵件以分析傳遞時寄件者的電子郵件驗證失敗;可在一天內取得結果。 

如果您擁有傳送基礎結構，請複查如何將它與 SPF、DKIM 及 DMARC 對齊，以確保目的地電子郵件系統信任從您網域傳送的郵件。 或者，請與寄件者聯繫，以解決其 DNS 設定。

**Microsoft 篩選 verdicts** 這部分在您的控制項中以進行修正。

提交郵件，並將郵件報告為安全;在一天內可重新掃描結果。 當您在特定情況下反對使用篩選 verdicts 時，請使用承租人允許/封鎖清單。 不過，您不應永久略過 Microsoft 篩選 verdicts。 

如需詳細資訊，請參閱：

- 讓您的使用者能夠將郵件提交給 Microsoft。 Microsoft 會使用這些報送，以提升電子郵件保護技術的效能，並顯示在提交報告中，供您用來做為更新原則的指示。 

- 若要在提交郵件進行分析時觀看簡短的影片，請參閱 [提交郵件進行分析](https://go.microsoft.com/fwlink/?linkid=2166435)。

- [使用系統管理提交，將可疑的垃圾郵件、網路釣魚詐騙、URL 和檔案提交給 Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [管理租用戶允許/封鎖清單](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Microsoft 365 的反垃圾郵件標頭](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [EOP 中的外寄垃圾郵件保護](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)