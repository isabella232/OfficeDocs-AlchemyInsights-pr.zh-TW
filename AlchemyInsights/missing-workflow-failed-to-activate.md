---
title: 無法啟動遺失的工作流程
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667077"
---
# <a name="missing-workflow-failed-to-activate"></a>無法啟動遺失的工作流程

在 Microsoft SharePoint 網站集合中，您無法新增全域可重複使用的工作流程 (例如「核准-SharePoint 2010」 ) 至清單或文件庫。
  
若要解決此問題，請遵循下列步驟： 
  
1. 在 SharePoint 設計工具2013中開啟網站集合的根網站。
  
2. 在 [ **網站物件**] 底下，選取 [ **工作流程**]。 
  
3. 在 [**工作流程**] 功能區的**新**區段中，選取 [**可重複使用的工作流程**] 
  
4. 在 [ **建立可重複使用的工作流程** ] 表單上，輸入名稱 * * *Repair2010* * *。 針對 [ **平臺類型**]，按一下 [ **SharePoint 2010 工作流程**]，然後按一下 **[確定]**。 
  
1. 在 [**工作流程**] 功能區的 [**儲存**] 區段中，選取 [**發佈**]。 
  
2. 在 [**工作流程**] 功能區的 [**管理**] 區段中，選取 [**全域發佈**]。 在出現的確認對話方塊中，選取 **[確定**]。 
  
3. 在網頁瀏覽器中，找出網站集合的根網站，然後存取 **網站設定** \> **網站集合的功能**。 然後，切換 **工作流程** 功能： 
  
·如果已  *啟用*  該功能，請按一下 [ **停用]，** 然後按一下 [ **啟動**]。 
  
·如果  *停用*  此功能，請按一下 [ **啟動**]。 
  
如需詳細資訊，請參閱下列 [文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。
  

