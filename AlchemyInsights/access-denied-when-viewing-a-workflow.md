---
title: 在查看工作流程時存取遭到拒絕
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955192"
---
# <a name="access-denied-when-viewing-a-workflow"></a>在查看工作流程時存取遭到拒絕

如果 SharePoint 群組的成員資格未設定為 [所有人]，則 SharePoint 2013 嘗試將電子郵件傳送至 SharePoint 群組的工作流程會失敗，並顯示「拒絕存取」錯誤訊息。
  
 **若要解決此問題，請執行下列步驟：**
  
 1. 允許所有人查看 SharePoint 群組的成員。
  
 2. 從電子郵件的 [收件者] 或 [抄送] 行中移除 SharePoint 群組。
  
 3. 如果無法變更 SharePoint 群組的成員資格可見度，請明確將使用者新增至 [收件者] 或 [副本] 行。
  
若要查看更多詳細資料 [，請參閱 HTTP 未經授權的/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)。
  