---
title: 磁碟機對應至 SharePoint 時，拒絕存取
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737468"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="dd310-102">修正 SharePoint 文件庫對應網路磁碟機的問題</span><span class="sxs-lookup"><span data-stu-id="dd310-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="dd310-103">當您瀏覽至對應的網路磁碟機時，您可能會看到下列其中一個下列訊息：</span><span class="sxs-lookup"><span data-stu-id="dd310-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="dd310-104">**\\無法存取路徑。您可能沒有使用此網路資源的權限。請連絡此伺服器的管理員，以找出是否您有存取權限。**</span><span class="sxs-lookup"><span data-stu-id="dd310-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="dd310-105">**拒絕存取。之前在此位置開啟檔案，您必須先將網站新增至信任的網站清單，瀏覽至網站，並選取自動登入選項。**</span><span class="sxs-lookup"><span data-stu-id="dd310-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="dd310-106">[協助疑難排解對應網路磁碟機](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。</span><span class="sxs-lookup"><span data-stu-id="dd310-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="dd310-107">對應網路磁碟機為文件庫會暫時和支援只能在 Internet Explorer 中。</span><span class="sxs-lookup"><span data-stu-id="dd310-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="dd310-108">相反地，[同步處理 SharePoint 檔案與新的 OneDrive 同步處理用戶端](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)包括[檔案隨選](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)。</span><span class="sxs-lookup"><span data-stu-id="dd310-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="dd310-109">存取您在 OneDrive 中的所有檔案，而不使用本機儲存空間。</span><span class="sxs-lookup"><span data-stu-id="dd310-109">Access all your files in OneDrive without using local storage space.</span></span>
  