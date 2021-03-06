---
title: 自動加密某些 Office 365 電子郵件
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509911"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>自動加密某些 Office 365 電子郵件

您可以自動加密使用者傳送給特定外部人員或組織的郵件。 若要執行此動作，請執行下列步驟：

1. 從 [Exchange 系統管理中心](https://outlook.office365.com/ecp/)，選擇 [ **郵件流程] > 規則**。 
2. 按一下 [ **新 (+)** ] 圖示，然後按一下 [套用 **Office 365 郵件加密和許可權保護至郵件**]。
3. 在 [ **名稱**] 中，輸入規則的名稱，例如 [ *加密傳送至 DrToniRamos@gmail.com 的郵件*]。
4. 在 [套用 **此規則**] 中，選擇 **[收件者] > 為此人員**。 
5. 在 [ **選取成員** ] 視窗中，選取您要套用加密規則的人員名稱，然後按一下 [ **新增**]。 
6. 當您完成新增使用者時，請按一下 **[確定]**。
7. 在 [ **執行下列** 欄位] 旁，按一下 [ **選取一個**]。 
8. 在 [ **RMS 範本** ] 下拉式功能表中，選取 [ **加密**]，然後按一下 **[確定]**。  (如果您沒有看到此選項，則表示您的計畫不包含自動加密。 不過，您可以新增！ ) 
9. 從您可以在此位置進行的選用選項清單中選擇任何選擇性選擇 (，許多可以保留預設設定為簡潔性) 。
10. 按一下 **[儲存]**。

> [!IMPORTANT]
> 您隨時可以傳回和編輯此規則。

如需建立加密規則的相關資訊，請參閱 [定義郵件流程規則，以加密 Office 365 中的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。

