---
title: 資料位置
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627837"
---
# <a name="data-location"></a>資料位置

在系統管理中心或連線到 Exchange Online 透過 PowerShell，您可以檢視您的 Office 365 租用戶的位置。


**系統管理中心：**
1. 登入[系統管理中心](https://admin.microsoft.com/Adminportal/Home)。
2. 選取 [**設定** > **組織設定檔**。
3. 在 [**資料位置**]，選取 [**檢視詳細資料**]。


**PowerShell:**
1. 使用 Windows PowerShell 連線到 Exchange Online。
2. 執行[Get-organizationalunit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit)指令程式，來顯示您的租用戶內容的清單。 
3. 查看 OrganizationId 屬性。

當您有 EXO 和 SPO 的資料位置時，您可以判斷您可能會從[您的資料所在的位置](https://products.office.com/where-is-your-data-located)使用其他服務的資料位置。