---
title: 自動加密 office 365 的特定電子郵件
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988826"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>自動加密 office 365 的特定電子郵件

1. 從 [Exchange 系統管理中心](https://outlook.office365.com/ecp/)，選擇 [**郵件流程] > 規則**]。 
2. 按一下 [**新 (+)** ] 圖示，然後按一下 [套用 **Office 365 郵件加密和許可權保護至郵件**]。
3. 在 [ **名稱**] 中，輸入規則的名稱，例如 [ *加密所有郵件*]。
4. 在 [套用 **此規則**] 中，選擇 **[套用至所有郵件]**。 
5. 在 [ **執行下列** 欄位] 旁，按一下 [ **選取一個**]。 
6. 在 [ **RMS 範本** ] 下拉式功能表中，選取 [ **加密**]，然後按一下 **[確定]**。  (如果您沒有看到此選項，則表示您的計畫不包含自動加密。 不過，您可以新增！ ) 
7. 選取 [ **以嚴重性層級審核此規則** ] 核取方塊，然後選取所需的層級。 如果貴公司有合約，將所有電子郵件都傳送給所有電子郵件，建議將層級設為 **高**。
8. 在 **[選擇此規則的模型**] 底下，按一下 [ **強制**]。 
9. 從您可以在此位置進行的選用選項清單中選擇任何選擇性選擇 (，許多可以保留預設設定為簡潔性) 。
10. 按一下 **儲存**。

> [!IMPORTANT]
> 您隨時可以傳回和編輯此規則。

如需建立加密規則的相關資訊，請參閱[定義郵件流程規則，以加密 Office 365 中的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

