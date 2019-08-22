---
title: 將外部使用者新增至通訊群組
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494518"
---
# <a name="add-external-users-to-a-distribution-group"></a>將外部使用者新增至通訊群組？

新增外部連絡人至通訊群組 (DG) 是 2 雙步驟程序：
  
1. 建立郵件連絡人的外部使用者：
    
    1. 在系統管理中心，移至 [**使用者** > [連絡人](https://admin.microsoft.com/adminportal/home#/Contact)] 頁面。 
    
    2. 選取 [**新增連絡人**。
    
    3. 輸入您的連絡人資訊，然後選取 [**新增]**。
    
2. 將郵件連絡人新增至您 DG:
    
    1. 在系統管理中心，移至 [**群組** > [群組](https://admin.microsoft.com/adminportal/home#/groups)] 頁面。 
    
    2. 尋找您想要將外部使用者加入，的 DG，然後選取 [以開啟 [編輯] 對話方塊。
    
    3. 在 [**成員**] 索引標籤中，選取 [**檢視所有及管理成員**。 
    
    4. 選取 [**新增成員**。
    
    5. 選取您在前一個步驟中，建立郵件連絡人，然後選取 [**儲存**。
    
如果執行這些步驟之後您的外部使用者無法傳送電子郵件給 DG，或未收到電子郵件從它，它可能是 DG 被標記為僅允許來自內部使用者的 [電子郵件。 您可以檢查此組態並修正下列指示[以下](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)。
  
 **附註：** 這些指示不適用，如果您的群組類型是 「 Office 365 群組 」 而不是 「 通訊群組 」。 如果是這種情況，您可以直接對群組新增外部使用者，從 Outlook 項目。 在 Office 365 群組來賓的詳細的資訊以及指示新增外部訪客可以在[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)中找到。
  