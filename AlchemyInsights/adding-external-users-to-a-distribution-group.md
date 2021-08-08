---
title: 將外部使用者新增至通訊群組
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934824"
---
# <a name="add-external-users-to-a-distribution-group"></a>將外部使用者新增至通訊群組

將外部連絡人新增至通訊群組 (DG) 分兩個步驟的程式：
  
1. 為外部使用者建立郵件連絡人：
    
    1. 在系統管理中心中，移至 [**使用者**  >  [連絡人](https://admin.microsoft.com/adminportal/home#/Contact)] 頁面。 
    
    2. 選取 [ **新增連絡人**]。
    
    3. 輸入您的連絡人資訊，然後選取 [ **新增**]。
    
2. 將郵件連絡人新增至您的 DG:
    
    1. 在系統管理中心中，移至 [**群組**  >  [群組](https://admin.microsoft.com/adminportal/home#/groups)] 頁面。 
    
    2. 尋找您要新增外部使用者的 DG，然後選取該 DG 以開啟 [編輯] 對話方塊。
    
    3. 在 [ **成員** ] 索引標籤上，選取 [ **全部查看] 和 [管理成員**]。 
    
    4. 選取 [新增成員]。
    
    5. 選取您在上一個步驟中建立的郵件連絡人，然後選取 [ **儲存**]。
    
遵循這些步驟之後，您的外部使用者無法將電子郵件傳送至 DG，或是未接收到該 DG 的電子郵件，可能是該 DG 已標示為只允許來自內部使用者的電子郵件。 您可以檢查此設定，並在 [這裡](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)遵循下列指示加以修正。
  
 **附注：** 如果您的群組類型是「Microsoft 365 group」，而不是「通訊群組」，這些指示將不適用。 如果是這種情況，您可以從 Outlook 將外部使用者直接新增至群組。 如需 Microsoft 365 群組來賓的詳細資訊，以及新增外部來賓的指示，請參閱[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)。
  