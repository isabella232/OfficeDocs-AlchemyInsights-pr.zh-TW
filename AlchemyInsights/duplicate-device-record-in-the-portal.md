---
title: 入口網站中的重複裝置記錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814507"
---
# <a name="duplicate-device-record-in-the-portal"></a>入口網站中的重複裝置記錄

如果裝置未正確將共同管理狀回報給 Configuration Manager 網站，您可能會在入口網站看到 2 筆裝置記錄。 若要檢查裝置的共同管理狀態，請在 Configuration Manager 主控台中查看該裝置 [Co-managed] 欄。 如果看不到該欄，您可以直接以滑鼠右鍵按一下任一欄標題，然後從清單中選取來新增欄。

Co-managed 值必須為 [是]。 如果該值是 [否]，請在用戶端裝置上開啟 Configuration Manager 用戶端小程式，然後在 [一般] 索引標籤中核取 **Co-management** 屬性。

- 如果此值為 [已啟用]，表示問題出在用戶端與管理點間的通訊。 請查看裝置上的 **CcmMessaging.log**，以調查可能的連線問題。

- 如果值為 [已停用] 且裝置已在 Intune 中註冊，請查看裝置上的 **CoManagementHandler.log**，以確保裝置收到共同管理原則。
