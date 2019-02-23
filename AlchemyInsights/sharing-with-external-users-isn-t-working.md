---
title: 與外部使用者共用也無法正常運作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207676"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>修正問題與外部使用者共用 SharePoint 內容

請確定外部共用您的組織已開啟：
  
1. 移至 [[服務&amp;增益集] 頁面上的 Microsoft 365 系統管理中心](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，並按一下 [**網站**]。
    
2. 確定設定開啟以 「 開啟 」。如果已選取 「 唯一現有外部使用者 」，請確認外部使用者會列於 Microsoft 365 系統管理中心。
    
確定外部共用其開啟網站。傳統的網站集合：
  
1. 在傳統 SharePoint 系統管理中心，在左窗格中，按一下 [**網站集合**]。
    
2. 選取網站] 或 [網站]，並在功能區] 上按一下 [**共用**]。
    
Office 365] 群組中，屬於小組網站或通訊網站：
  
- 這些新的網站類型具有相同共用將設為您的整個組織的設定，除非整個組織的設定可讓共用檔案使用不需要登入的連結。在此例中，網站會允許共用與新的和現有外部使用者登入。若要變更特定網站的設定，請使用新的 SharePoint 系統管理中心 （預覽） 或 PowerShell。[解更多](https://go.microsoft.com/fwlink/?linkid=871863)。
    
> [!NOTE]
> 外部共用任何網站的設定可以更嚴格比在整個組織設定，但不是更寬鬆比全組織設定。 
  

