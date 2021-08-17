---
title: 修正連接原則
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
- "9000760"
- "7391"
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888397"
---
# <a name="fix-connection-policy"></a>修正連接原則

電子郵件已標示為安全，並傳遞至使用者的收件匣，因為來源 IP 位址已標示為安全的預設連線篩選原則。 若要查看原則，請執行下列步驟：

1. 在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com/> ，移至 [**電子郵件 &** 共同作業 \> **原則] & 規則** \> 的 [原則] 區段中的 [**威脅原則** \> **反垃圾郵件**]。 

   若要直接移至 [反垃圾郵件原則 **]** 頁面，請使用 <https://security.microsoft.com/antispam>。

2. 在 [ **反垃圾郵件原則** ] 頁面上，透過按一下原則名稱，選取名為「連線 **篩選原則 (的原則預設)** 。

3. 在出現的 [詳細資料] 浮出視窗中，按一下 [連線 **篩選**] 區段中的 [**編輯連線篩選原則**]。

4. 查看 [ **無條件允許來自下列 IP 位址或位址範圍的郵件** ] 區段中的專案，然後查看是否已選取 [ **開啟安全清單** ]。

   > [!NOTE]
   > Microsoft 會訂閱協力廠商來源的信任寄件者。 如果啟用 [安全清單]，這些受信任的寄件者不會錯誤地標示為垃圾郵件。 建議您選取此選項，因為它會減少誤報數目 (很棒的郵件會被分類為您收到的垃圾郵件) 。

如需詳細資訊，請參閱[設定連線篩選](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)。
