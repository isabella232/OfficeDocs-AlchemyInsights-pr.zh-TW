---
title: 有關如何使用 Office 部署工具 (ODT) 的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774882"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>有關如何使用 Office 部署工具 (ODT) 的問題

從[Microsoft 下載中心](https://go.microsoft.com/fwlink/p/?LinkID=626065)下載 Office 部署工具。
  
下載檔案之後，執行自我解壓縮可執行檔，其中包含 Office 部署工具可執行檔 (setup.exe) 及範例組態檔 (configuration.xml)。
  
 **若要排除或移除用戶端電腦的 Microsoft 365 應用程式企業版產品：**
  
安裝適用于企業的 Microsoft 365 應用程式時，您可以排除特定產品。 方法是依照利用 ODT 安裝 Office 的步驟進行，但在組態檔中加入 ExcludeApp 元素。 例如，此設定檔案會為所有 Microsoft 365 應用程式安裝企業產品（Publisher 除外）：
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office 部署工具概觀](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

