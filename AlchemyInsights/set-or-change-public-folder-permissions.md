---
title: 設定或變更公用資料夾許可權
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: 1868b8b04df012d44781f86ee75120ca443af5be5801074329f17c0e40a5acc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060883"
---
# <a name="permissions-and-public-folders"></a>許可權和公用資料夾

您可以使用 Outlook、Exchange 系統管理中心 (EAC) 或 PowerShell: 來變更公用資料夾的許可權。
  
- 如需 Outlook 指示，請[按一下這裡](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)。
    
- 若為 EAC，請參閱 [本文](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) 以取得相關指示。 
    
- 如需 Powershell，請參閱 [本文](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) ，以取得使用 Add-PublicFolderClientPermission commandlet 的指示。 如果您需要指示連接至 Exchange Powershell，請按一下[這裡](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)。
    
如果 **外部使用者無法將電子郵件傳送至擁有郵件功能的公用資料夾**，原因可能是公用資料夾缺少外部電子郵件傳遞所需的許可權。 您可以使用[這裡](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)的 Outlook 指示來修正此問題，或在[這裡](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)PowerShell 指示。
  

