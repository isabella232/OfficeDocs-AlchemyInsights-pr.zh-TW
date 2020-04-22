---
title: 將磁片對應至 SharePoint 時，存取權遭到拒絕
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687357"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="91d77-102">修正對應至網路磁碟機的 SharePoint 程式庫的問題</span><span class="sxs-lookup"><span data-stu-id="91d77-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="91d77-103">當您流覽到對應的網路磁碟機時，可能會出現下列其中一則訊息：</span><span class="sxs-lookup"><span data-stu-id="91d77-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="91d77-104">**\\無法存取路徑。您可能沒有使用此網路資源的許可權。請洽詢此伺服器的管理員，以找出您是否有存取許可權。**</span><span class="sxs-lookup"><span data-stu-id="91d77-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="91d77-105">**拒絕存取。在此位置開啟檔案之前，您必須先將網站新增至信任的網站清單，流覽至網站，然後選取 [自動登入] 選項。**</span><span class="sxs-lookup"><span data-stu-id="91d77-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="91d77-106">[取得協助疑難排解對應的網路磁碟機](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。</span><span class="sxs-lookup"><span data-stu-id="91d77-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="91d77-107">將文件庫對應為網路磁碟機，只會在 Internet Explorer 中進行暫存和支援。</span><span class="sxs-lookup"><span data-stu-id="91d77-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="91d77-108">相反地，請[使用新的 OneDrive 同步用戶端](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)（包括所[需的](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)檔案）同步處理 SharePoint 檔案。</span><span class="sxs-lookup"><span data-stu-id="91d77-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="91d77-109">在 OneDrive 中存取所有檔案，而不使用本機儲存空間。</span><span class="sxs-lookup"><span data-stu-id="91d77-109">Access all your files in OneDrive without using local storage space.</span></span>
  