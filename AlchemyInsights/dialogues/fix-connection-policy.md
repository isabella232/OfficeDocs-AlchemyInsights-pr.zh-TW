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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568495"
---
# <a name="fix-connection-policy"></a>修正連接原則

電子郵件已標示為安全，並傳遞至使用者的收件匣，因為在連線篩選原則中已標示為安全的傳送 IP 位址。 若要查看原則，請執行下列操作：

1. 移至 [Office 365 Security & 合規性中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)，然後移至 **威脅管理**  >  **原則**  >  [反垃圾郵件](https://go.microsoft.com/fwlink/?linkid=2101518)。
2. 在 [ **自訂** ] 索引標籤上，選取連線 **篩選原則**，然後選取 [ **編輯原則**]。
3. 複查 [ **IP 允許** ] 清單。 請參閱是否已啟用 **安全清單** 。

    > [!NOTE]
    > Microsoft 會訂閱協力廠商來源的信任寄件者。 如果啟用 **安全清單** ，這些受信任的寄件者不會錯誤地標示為垃圾郵件。 我建議選取此選項，因為它會減少誤報數目 (很棒的郵件會被分類為您收到的垃圾郵件) 。
