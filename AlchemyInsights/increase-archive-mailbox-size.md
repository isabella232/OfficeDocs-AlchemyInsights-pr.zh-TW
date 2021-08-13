---
title: 305增加封存信箱大小
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f9cc968aba32645fd4433616618d096231ce4899e9e93335e802af5c05524a79
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926374"
---
# <a name="increase-the-archive-mailbox-size"></a>增加封存信箱大小


如果您想讓我們為下列所述的設定執行自動檢查，請選取此頁面頂端的 [上一步] 按鈕 <--然後輸入需要增加其封存信箱大小的使用者電子郵件地址。

Microsoft 365 會根據指派給使用者帳戶的授權，[限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)封存信箱的大小。 當封存信箱達到其允許大小的90% 時，使用者會收到電子郵件通知。 當封存信箱達到其大小限制時，使用者就無法將更多專案移至封存信箱。 達到大小限制時，Microsoft 365 不會增加封存信箱的大小。 相反地，使用者可以採取下列動作來釋放封存信箱中的空間：

- 使用 Outlook 將專案匯出為 .pst 檔案。

- 刪除封存信箱中的專案。

Microsoft 365 為 Office 365 企業版 E3 和 E5 授權提供 **無限期** 的封存。 管理員必須啟用此功能，封存信箱才能達到其大小上限。 當無限期封存啟用時，最多可能需要30天才能將可用空間新增至封存信箱。 因此，建議系統管理員驗證封存信箱中的可用空間，讓使用者可以在展開時繼續使用封存信箱。 如需詳細資訊，請參閱[Microsoft 365 中的無限](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)封存，並[在 Microsoft 365 中啟用無限](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)封存。

如需從 Outlook 存取封存信箱的詳細資訊，請參閱[在自動展開的封存中存取專案 Outlook 需求](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)。 若要設定自動將專案移至封存信箱的保留原則，請參閱[設定 Microsoft 365 組織中信箱的封存和刪除原則](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)。

**附注**： Exchange 2010 上的主要信箱不支援自動展開的封存。
