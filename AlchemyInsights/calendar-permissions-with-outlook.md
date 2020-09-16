---
title: 行事曆許可權
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748784"
---
# <a name="calendar-permissions"></a><span data-ttu-id="f3d5f-102">行事曆許可權</span><span class="sxs-lookup"><span data-stu-id="f3d5f-102">Calendar Permissions</span></span>

<span data-ttu-id="f3d5f-103">使用者可以使用網頁或其他用戶端上的 Outlook 變更自己的行事曆許可權，但您也可能需要調查的系統管理員。</span><span class="sxs-lookup"><span data-stu-id="f3d5f-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="f3d5f-104">使用 Exchange PowerShell Cmdlet 會向您顯示使用者行事曆的許可權：</span><span class="sxs-lookup"><span data-stu-id="f3d5f-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="f3d5f-105">若要查看詳細資訊，請參閱下列各項：</span><span class="sxs-lookup"><span data-stu-id="f3d5f-105">To see more information see the following:</span></span>

- [<span data-ttu-id="f3d5f-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="f3d5f-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="f3d5f-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="f3d5f-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="f3d5f-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="f3d5f-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="f3d5f-109">行事曆許可權用於共用的行事曆中，若要查看有關共用 Outlook 行事曆的詳細資訊，請參閱下列文章：</span><span class="sxs-lookup"><span data-stu-id="f3d5f-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="f3d5f-110">與其他人共用 Outlook 行事曆</span><span class="sxs-lookup"><span data-stu-id="f3d5f-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="f3d5f-111">在商務用 Outlook 網頁版中共用您的行事曆</span><span class="sxs-lookup"><span data-stu-id="f3d5f-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="f3d5f-112">若要疑難排解「行事曆」許可權，您可以使用 [支援和修復助理](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) 工具。</span><span class="sxs-lookup"><span data-stu-id="f3d5f-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>