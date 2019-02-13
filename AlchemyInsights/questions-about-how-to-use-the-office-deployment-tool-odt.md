---
title: 如何使用 Office 部署工具 (ODT) 相關的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925335"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="bea93-102">如何使用 Office 部署工具 (ODT) 相關的問題</span><span class="sxs-lookup"><span data-stu-id="bea93-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="bea93-103">從[Microsoft 下載中心](http://go.microsoft.com/fwlink/p/?LinkID=626065)下載 Office 部署工具。</span><span class="sxs-lookup"><span data-stu-id="bea93-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="bea93-104">下載檔案之後，執行自我解壓縮可執行檔，其中包含 Office 部署工具可執行檔 (setup.exe) 及範例組態檔 (configuration.xml)。</span><span class="sxs-lookup"><span data-stu-id="bea93-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="bea93-105">**若要排除或移除的用戶端電腦的 Office 365 ProPlus 的產品：**</span><span class="sxs-lookup"><span data-stu-id="bea93-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="bea93-p101">安裝 Office 365 專業增強版時，您可以排除特定產品。若要這麼做，請遵循使用 ODT 安裝 Office 的步驟，但是在您的組態檔中包含 ExcludeApp 元素。例如，這個組態檔會安裝「發行者」以外的所有 Office 365 專業增強版產品︰</span><span class="sxs-lookup"><span data-stu-id="bea93-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="bea93-109">Office 部署工具概觀</span><span class="sxs-lookup"><span data-stu-id="bea93-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

