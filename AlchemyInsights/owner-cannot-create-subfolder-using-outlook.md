---
title: 擁有者無法使用 Outlook 建立子資料夾
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836126"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>擁有者無法使用 Outlook 建立子資料夾

**公用資料夾擁有者使用 Outlook 建立子資料夾時發生一個持續存在的問題。我們將盡快修正此問題。**

在此同時，您可以使用下列因應措施：

1. 使用 MAC 版 Outlook 建立子資料夾，因為這個問題只會影響電腦版 Windows 的 Outlook (所有版本)
2. 讓系統管理員使用 EXO Shell 或 EAC 建立子資料夾
3. 將使用者的 DefaultPublicFolderMailbox/EffectivePublicFolderMailbox 變更為造成問題之資料夾的內容信箱以外的其他信箱  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. 等候一小時，重新啟動 outlook 用戶端