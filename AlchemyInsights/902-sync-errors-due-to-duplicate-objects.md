---
title: 902 （重複物件由於同步處理錯誤）
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919863"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>重複物件由於同步處理錯誤

您可能會收到下列錯誤訊息的其中一個目錄同步作業完成時：
  
- 無法更新此物件的 Microsoft Online Services 因為此物件相關聯的下列屬性的可能已經與您的本機目錄中的其他物件相關聯的值。
    
- 您的 Microsoft Online Services 目錄中已經存在具有相同的 proxy 地址的同步處理的物件。
    
- 無法更新此物件因為此物件相關聯的下列屬性的可能已經與您的本機目錄服務中的其他物件相關聯的值： UserPrincipalName。
    
若要找出並修正的問題，下載和執行[IdFix DirSync 錯誤補救工具](https://www.microsoft.com/download/details.aspx?id=36832)。
  
如需詳細資訊，請參閱[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。
  

