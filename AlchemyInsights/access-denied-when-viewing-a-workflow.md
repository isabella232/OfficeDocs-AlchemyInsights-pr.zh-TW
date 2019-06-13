---
title: 檢視工作流程時，拒絕存取
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883582"
---
# <a name="access-denied-when-viewing-a-workflow"></a>檢視工作流程時，拒絕存取

如果 SharePoint 群組的成員資格不設為所有人，嘗試將電子郵件傳送至 SharePoint 群組的 SharePoint 2013 工作流程可能會失敗與 「 存取被拒 」 錯誤訊息。
  
 **若要解決此問題，請執行下列步驟：**
  
 1. 允許所有人都可以查看 SharePoint 群組的成員。
  
 2. SharePoint 群組移除 [收件者] 或 [副本] 行的電子郵件。
  
 3. 明確地將使用者新增至 [收件者] 或 [副本] 行如果無法變更 SharePoint 群組成員資格可見性。
  
若要檢視的詳細資訊請參閱[HTTP 未經授權至 /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。
  