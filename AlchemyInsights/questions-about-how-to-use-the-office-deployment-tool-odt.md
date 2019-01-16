---
title: 如何使用 Office 部署工具 (ODT) 相關的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278224"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>如何使用 Office 部署工具 (ODT) 相關的問題

從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載 Office 部署工具。
  
下載檔案之後，執行自我解壓縮可執行檔，其中包含 Office 部署工具可執行檔 (setup.exe) 及範例組態檔 (configuration.xml)。
  
 **若要排除或移除的用戶端電腦的 Office 365 ProPlus 的產品：**
  
安裝 Office 365 專業增強版時，您可以排除特定產品。若要這麼做，請遵循使用 ODT 安裝 Office 的步驟，但是在您的組態檔中包含 ExcludeApp 元素。例如，這個組態檔會安裝「發行者」以外的所有 Office 365 專業增強版產品︰
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office 部署工具概觀](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

