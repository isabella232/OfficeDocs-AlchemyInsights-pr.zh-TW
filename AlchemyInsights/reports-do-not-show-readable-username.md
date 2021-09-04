---
title: Microsoft 365 系統管理中心的報告未顯示可讀取的使用者名稱
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2021
ms.locfileid: "58896345"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Microsoft 365 系統管理中心的報告未顯示可讀取的使用者名稱

Microsoft 365 系統管理中心的報告不會顯示使用者名稱，而是顯示英數字元值，例如 B2BC6C15BB9FCDEA71E5CD302D228CC8。

這是預期的行為，已在訊息中心傳達 (MC275344，2021 年 8 月 3 日發佈)。 

全域系統管理員可以為其租用戶還原此變更，並顯示可識別的使用者資訊 (如果其組織隱私權實務允許)。若要還原租用戶變更：

1. 在系統管理中心中，前往 **[設定]**  > **[組織設定]** > [**[服務]**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)，然後選取 **[報告]**。 
1. 在 [選擇如何顯示使用者資訊]**** 下，選取 [在報告中顯示可識別的使用者資訊 **]**，然後重新執行報告。