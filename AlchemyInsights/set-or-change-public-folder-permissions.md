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
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32421807"
---
# <a name="permissions-and-public-folders"></a>權限及公用資料夾

您可以使用 Outlook，Exchange 系統管理中心 (EAC) 中，將公用資料夾上變更權限或 PowerShell:
  
- Outlook 的指示，[請按一下這裡](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)。
    
- EAC 中，請參閱[這篇文章](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1)的指示。 您可以按一下[這裡](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx)瀏覽至 EAC。 
    
- Powershell 中，請參閱[這篇文章](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx)說明如何使用 Add-publicfolderclientpermission commandlet。 如果您需要連線到 Exchange Powershell 的指示，請按一下[這裡](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)。
    
如果**外部使用者將無法傳送電子郵件至擁有郵件功能的公用資料夾**，原因可能是公用資料夾遺漏的權限所需的外部電子郵件傳遞。 您可以修正這使用 Outlook 指示在[這裡](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)，或 PowerShell 指示[以下](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)。
  

