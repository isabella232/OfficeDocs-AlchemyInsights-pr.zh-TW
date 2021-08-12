---
title: 與外部使用者共用無法運作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910357"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>修正與外部使用者 SharePoint 內容共用的問題

請確定您的組織已開啟外部共用：
  
1. 移至 [Microsoft 365 系統管理中心中的 [服務 &amp; 增益集] 頁面](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，然後按一下 [**網站**]。
    
2. 確定設定已開啟「開啟」。 如果選取 [只是現有的外部使用者]，請確定外部使用者已列在 Microsoft 365 系統管理中心中。
    
請確定網站已開啟外部共用。 針對傳統網站集合：
  
1. 在 [新增 SharePoint 系統管理中心] 的左窗格中，按一下 [**網站**]。
    
2. 選取網站，然後按一下功能區上的 [ **共用**]。
    
針對屬於 Microsoft 365 群組或通訊網站的小組網站：
  
- 這些新網站類型與整個組織設定具有相同的共用設定，除非整個組織設定允許使用不需要登入的連結來共用檔案。 在此情況下，網站允許與新的和現有的外部使用者共用登入。 若要變更特定網站的設定，請使用新 SharePoint 系統管理中心或 PowerShell。 [深入了解](https://go.microsoft.com/fwlink/?linkid=871863)。
    
> [!NOTE]
> 任何網站的外部共用設定，都比整個組織的設定更具限制性，但不如整個組織的設定。 
  

