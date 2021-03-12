---
title: 自動將電子郵件移至封存信箱
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735998"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>自動將電子郵件移至封存信箱

以下說明如何設定原則，以自動將使用者的舊電子郵件移至封存信箱：

1. 移至 [**安全性 & 合規性**](https://go.microsoft.com/fwlink/p/?linkid=2077143)資料控管封存  >    >   ，以確認使用者已啟用封存信箱。 若尚未使用，按一下 [警告] 方塊中的 [ **啟用** ]，然後按一下 [ **是]** 。
2. 移至 [**Exchange 系統管理中心 > 合規性管理 > 保留標記**](https://go.microsoft.com/fwlink/?linkid=2059104)。
3. 選擇 [+] 圖示，然後選擇 [ **自動套用至整個信箱**]。
4. 將名稱指派給保留標記，然後選擇 [ **移至** 封存]。 在保留期間內，輸入您想要的時間，例如90天。 按一下 **[儲存]**。
5. 現在建立保留原則：選擇 [ **保留** 原則]，然後選擇圖示以新增原則。
6. 將名稱指派給保留原則，然後按一下和滾動以尋找並新增您剛才建立的保留標記。 按一下 **[儲存]**。
7. 最後，將保留原則套用至使用者的信箱：仍然在 Exchange 系統管理中心中，移至 [收件者] **[信箱]**  >  ****。 選擇您要套用原則的所有使用者，然後選擇 [ **編輯** (鉛筆圖示) 。
8. 在對話方塊中，按一下 [ **信箱功能**]。 在 [ **保留原則**] 下，套用您剛才建立的原則 > **儲存**]。
9. 如需將原則套用至所有使用者的指示，請參閱 [將保留原則套用至信箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。
