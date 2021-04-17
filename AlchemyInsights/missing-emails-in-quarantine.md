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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831725"
---
# <a name="missing-emails-in-quarantine"></a>隔離中遺失的電子郵件 "

管理員可以 [查看、發行或刪除這些郵件。](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

若要開啟安全性 & 規範中心，請移至 [https://protection.office.com](https://protection.office.com/) 。 若要直接開啟 [隔離] 頁面，請移至 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。  

您可以依下列值進行搜尋：  

- **郵件識別碼**：郵件的全域唯一識別碼。 如果您選取清單中的訊息，[**詳細資料**] 彈出窗格中隨即會顯示 [**郵件識別碼**] 值。 系統管理員可以使用 [郵件追蹤][](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) 來尋找郵件及其對應的郵件識別碼值。
- **寄件者電子郵件地址**：單一寄件者的電子郵件地址。
- **收件者電子郵件地址**：單一收件者的電子郵件地址。
- **主旨**：使用郵件的完整主旨。 搜尋時不會區分大小寫。

輸入搜尋準則之後，請按一下 [重新整理按鈕重新整理] ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) 以篩選結果。  

您用來在隔離區中查看及管理郵件和檔案的 Cmdlet 如下：
- [Delete-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [預覽-get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)：請注意，此 Cmdlet 只適用于 SharePoint Online、商務 OneDrive 或小組的 ATP 中的電子郵件，而非惡意程式碼檔案。
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)