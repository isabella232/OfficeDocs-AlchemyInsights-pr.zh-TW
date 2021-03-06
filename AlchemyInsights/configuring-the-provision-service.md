---
title: 設定供給服務
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480745"
---
# <a name="configuring-the-provision-service"></a>設定供給服務

為了讓自動化的使用者布建能夠運作，Azure AD 需要有效的認證，以允許其連線至 Workday Web 服務 API。 此外，在 Workday 至 AD 使用者布建應用程式上的 [測試連線] 按鈕，也會驗證是否可以連線至與 AD 網域相關聯的 Azure AD Connect 布布布建代理程式。

如果 Azure 入口網站在儲存認證時傳回錯誤，請遵循下列建議步驟：

1. 請確認您已依照 [教學課程] 區段 [設定 workday 中的 Integration System 使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)所述，設定 Workday 整合系統使用者帳戶。
2. 請確認 Azure AD Connect 布建代理程式服務已啟動，且已在內部部署 Windows server 上使用服務管理主控台執行。 您也可以在 Azure 入口網站中，按一下 [查看內部部署代理程式] 按鈕，檢查代理程式的狀態。
3. 請務必使用 username@workday-租使用者名稱的格式，輸入 "Workday Username" 欄位的值。 如果 workday-租使用者名稱缺失，Workday 驗證會失敗。
4. 若要設定與 Workday 實施租使用者的整合，請注意 Workday 租使用者的排程停機時間。 Workday 的實施租使用者排定停機時間的期限超過週末 (通常從星期五晚上到星期六早上) 和此停機時間的連線失敗] 視窗是一種已知的問題，可在實施承租人傳回線上時自動解決。
5. 在極少的情況下，如果整合系統使用者的密碼因租使用者重新整理或帳戶處於鎖定或過期狀態，您也會看到此錯誤。 請使用 Workday 管理員檢查整合系統使用者的狀態。

如需有關設定 Workday 以自動佈建的詳細資訊，請參閱[教學課程：設定 Workday 來自動佈建使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。
