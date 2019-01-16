---
title: 檢視工作流程時拒絕存取
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278466"
---
# <a name="access-denied-when-viewing-a-workflow"></a>檢視工作流程時拒絕存取

如果 SharePoint 群組的成員資格] 未設為任何人使用 「 拒絕存取 」 錯誤訊息嘗試將電子郵件傳送至 SharePoint 群組的 SharePoint 2013 工作流程可能會失敗。
  
 **若要解決此問題，請執行下列步驟：**
  
 1. 可讓所有人都可以看到的 SharePoint 群組的成員。 
  
 2. SharePoint 群組移除 [收件者] 或 [副本] 行的電子郵件。 
  
 3. 明確地將使用者新增至 [收件者] 或 [副本] 行如果成員資格不能變更可見度 SharePoint 群組。 
  
若要檢視的詳細資訊請參考[HTTP 未經授權至 /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。
  

