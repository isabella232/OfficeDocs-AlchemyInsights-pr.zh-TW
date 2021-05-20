---
title: 隔離區中遺失的電子郵件
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539815"
---
# <a name="missing-emails-in-quarantine"></a>隔離中遺失的電子郵件 "

管理員可以 [查看、發行或刪除這些郵件。](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

若要開啟安全性 & 規範中心，請移至 [https://protection.office.com](https://protection.office.com/) 。 若要直接開啟 [隔離] 頁面，請移至 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。  

您可以依下列值進行搜尋：  

- **郵件識別碼**：郵件的全域唯一識別碼。 如果您選取清單中的訊息，[**詳細資料**] 彈出窗格中隨即會顯示 [**郵件識別碼**] 值。 系統管理員可以使用 [郵件追蹤][](/microsoft-365/security/office-365-security/message-trace-scc) 來尋找郵件及其對應的郵件識別碼值。
- **寄件者電子郵件地址**：單一寄件者的電子郵件地址。
- **收件者電子郵件地址**：單一收件者的電子郵件地址。
- **主旨**：使用郵件的完整主旨。 搜尋時不會區分大小寫。

輸入搜尋準則後，請按一下![重新整理按鈕](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) [重新整理] 來篩選結果。

您用來在隔離區中查看及管理郵件和檔案的 Cmdlet 如下：
- [Delete-Get-quarantinemessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-Get-quarantinemessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [預覽-get-quarantinemessage](/powershell/module/exchange/preview-quarantinemessage)：請注意，此 Cmdlet 只適用于來自 Microsoft Defender 的郵件，而不是 Microsoft Defender 的惡意程式碼檔案，以供 SharePoint Online、商務用 OneDrive 或 Teams 的 Office 365。
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)