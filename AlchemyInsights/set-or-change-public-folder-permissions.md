---
title: 設定或變更公用資料夾權限
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1015c2203406e15d6b418c387b6632a182d6d2ff
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36734660"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="15c7f-102">權限及公用資料夾</span><span class="sxs-lookup"><span data-stu-id="15c7f-102">Permissions and Public Folders</span></span>

<span data-ttu-id="15c7f-103">您可以使用 Outlook，Exchange 系統管理中心 (EAC) 中，將公用資料夾上變更權限或 PowerShell:</span><span class="sxs-lookup"><span data-stu-id="15c7f-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="15c7f-104">Outlook 的指示，[請按一下這裡](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)。</span><span class="sxs-lookup"><span data-stu-id="15c7f-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="15c7f-105">EAC 中，請參閱[這篇文章](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)的指示。</span><span class="sxs-lookup"><span data-stu-id="15c7f-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="15c7f-106">Powershell 中，請參閱[這篇文章](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)說明如何使用 Add-publicfolderclientpermission commandlet。</span><span class="sxs-lookup"><span data-stu-id="15c7f-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="15c7f-107">如果您需要連線到 Exchange Powershell 的指示，請按一下[這裡](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)。</span><span class="sxs-lookup"><span data-stu-id="15c7f-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="15c7f-108">如果**外部使用者將無法傳送電子郵件至擁有郵件功能的公用資料夾**，原因可能是公用資料夾遺漏的權限所需的外部電子郵件傳遞。</span><span class="sxs-lookup"><span data-stu-id="15c7f-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="15c7f-109">您可以修正這使用 Outlook 指示在[這裡](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)，或 PowerShell 指示[以下](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)。</span><span class="sxs-lookup"><span data-stu-id="15c7f-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

