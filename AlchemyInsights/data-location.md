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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655273"
---
# <a name="data-location"></a>資料位置

您可以在系統管理中心中查看租使用者的位置，或透過 PowerShell 連接至 Exchange Online。


**系統管理中心：**
1. 登入系統[管理中心](https://admin.microsoft.com/Adminportal/Home)。
2. 選取 [**設定** > **組織設定檔**]。
3. 在 [**資料位置**] 底下，選取 [**查看詳細**資料]。


**PowerShell:：**
1. 使用 Windows PowerShell 連接至 Exchange Online。
2. 執行[Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) Cmdlet 以顯示租使用者屬性的清單。 
3. 查看 OrganizationId 屬性。

當您有 EXO 和 SPO 的資料位置時，您可以判斷您的[資料所在位置](https://products.office.com/where-is-your-data-located)，您可以使用其他服務的資料位置。