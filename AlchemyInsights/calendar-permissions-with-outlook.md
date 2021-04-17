---
title: 行事曆許可權
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
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819899"
---
# <a name="calendar-permissions"></a>行事曆許可權

使用者可以使用網頁或其他用戶端上的 Outlook 變更自己的行事曆許可權，但您也可能需要調查的系統管理員。  
使用 Exchange PowerShell Cmdlet 會向您顯示使用者行事曆的許可權：

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

若要查看詳細資訊，請參閱下列各項：

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

行事曆許可權用於共用的行事曆中，若要查看有關共用 Outlook 行事曆的詳細資訊，請參閱下列文章：

- [與其他人共用 Outlook 行事曆](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [在商務用 Outlook 網頁版中共用您的行事曆](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

若要疑難排解「行事曆」許可權，您可以使用 [支援和修復助理](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) 工具。