---
title: 多個使用者在 Outlook 中沒有看見增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729862"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>多個使用者在 Outlook 中沒有看見增益集

如果您測試 Outlook 增益集而其並未顯示出來，疑難排解步驟一，請使用 **獲取-OrganizationConfig ** PowerShell Cmdlet 來查詢 _AppsForOfficeEnabled_ 參數。 如果查詢傳回 **[錯誤]** 值，請透過使用 **設定-OrganizationConfig** cmdlet 將參數設為 **[正確]**，這樣增益集就能正常顯示。

不建議將 _AppsForOfficeEnabled_ 參數設定為 **[錯誤]**。 **[錯誤]** 值會覆寫上述所有 [系統管理] 和 [使用者] 角色設定，並造成組織中的任何使用者無法啟用任何新的應用程式。

如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)。