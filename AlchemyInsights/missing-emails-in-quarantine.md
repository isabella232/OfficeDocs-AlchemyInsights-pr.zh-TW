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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329653"
---
# <a name="missing-emails-in-quarantine"></a>隔離區中遺失的電子郵件

管理員可以 [查看、發行或刪除這些郵件](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

在 Microsoft 365 Defender 入口網站上 <https://security.microsoft.com> ，移至 [**複查** \> **隔離區**]。 或者，若要直接移至 [ **隔離** ] 頁面，請使用 <https://security.microsoft.com/quarantine> 。  

如需您可以使用之搜尋/篩選值的詳細資訊，請參閱 [在 EOP 中，以系統管理員身分管理被隔離的郵件和](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)檔案。

您用來在隔離區中查看及管理郵件和檔案所用的 Cmdlet 如下：

- [Delete-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [預覽-get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)：請注意，此 Cmdlet 只適用于郵件，而不是 SharePoint、OneDrive 或 Microsoft Teams 的保管庫附件中的檔案。
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
