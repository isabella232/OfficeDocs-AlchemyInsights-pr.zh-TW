---
title: 唯讀方式開啟檔案
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6a828f8d-ff31-40a7-b701-b2339e771817
ms.openlocfilehash: 4c774864a03b7dbc099f64b7906fa4a0bc26c63c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525715"
---
# <a name="file-open-read-only"></a><span data-ttu-id="c4c6f-102">唯讀方式開啟檔案</span><span class="sxs-lookup"><span data-stu-id="c4c6f-102">File open read-only</span></span>

<span data-ttu-id="c4c6f-103">您可能會發現，當您開啟檔案，在開啟為唯讀。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="c4c6f-104">在某些情況下，是以提高安全性，例如當您從網際網路，以及其他時候開啟檔案，它可能是因為可以變更的設定。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="c4c6f-105">以下是唯讀檔案將會開啟其中某些情況下，若要變更此設定，可採取一些步驟。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="c4c6f-106">**我的防毒軟體會造成它們以唯讀方式開啟**</span><span class="sxs-lookup"><span data-stu-id="c4c6f-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="c4c6f-107">部分防毒程式可能會防止您具有潛在危險性的檔案開啟其唯讀屬性。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="c4c6f-108">您可能需要您防毒軟體的提供者了解如何調整這些設定，請洽詢。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="c4c6f-109">BitDefender，例如，具有上新增應用程式排除以下內容： [How to： 新增應用程式或處理程序排除 Bitdefender 控制項置中的](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl)。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="c4c6f-110">**檔案屬性設定為唯讀？**</span><span class="sxs-lookup"><span data-stu-id="c4c6f-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="c4c6f-111">您可以藉由將檔案上按一下滑鼠右鍵，然後選擇 [內容檢查檔案屬性。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="c4c6f-112">如果會檢查唯讀屬性，您可以取消選取它，然後按一下 [確定]。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="c4c6f-113">**內容位於受保護的檢視**</span><span class="sxs-lookup"><span data-stu-id="c4c6f-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="c4c6f-114">從網際網路和其他可能不安全位置的檔案可以包含病毒、 蠕蟲或其他類型的惡意程式碼會傷害您的電腦。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="c4c6f-115">這也是常與電子郵件附件或您已下載的檔案的情況。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="c4c6f-116">為了協助保護您的電腦，在受保護的檢視開啟檔案從這些可能不安全的位置。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="c4c6f-117">藉由使用受保護的檢視，您可以讀取檔案，並查看其內容，同時降低風險。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="c4c6f-118">如需有關受保護的檢視，以及如何變更設定的詳細資訊，請參閱這篇文章：[什麼是受保護的檢視？](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="c4c6f-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="c4c6f-119">**已滿 OneDrive？**</span><span class="sxs-lookup"><span data-stu-id="c4c6f-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="c4c6f-120">如果檔案儲存在 OneDrive 和您的 OneDrive 儲存空間已滿，將無法儲存文件，直到您受到分配的空間。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="c4c6f-121">您可以檢查您 OneDrive 上的可用空間，按一下通知中心中的 OneDrive 圖示，然後選擇 [管理存放區，或您可以移至[http://onedrive.live.com](http://onedrive.live.com)、 登入，並請注意畫面的左的使用中較低的空間量。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="c4c6f-122">**會在啟動 Office 嗎？**</span><span class="sxs-lookup"><span data-stu-id="c4c6f-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="c4c6f-123">如果不啟動 Office 時，或者如果您的訂閱已過期，您可能是以唯讀方式可精簡功能模式。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="c4c6f-124">如需如何啟用 Office 的資訊，請參閱：[未授權產品和啟用錯誤 Office 中的](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380)。</span><span class="sxs-lookup"><span data-stu-id="c4c6f-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/unlicensed-product-and-activation-errors-in-office-0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="c4c6f-125">**如果所有人失敗...]**</span><span class="sxs-lookup"><span data-stu-id="c4c6f-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="c4c6f-126">請嘗試重新啟動電腦</span><span class="sxs-lookup"><span data-stu-id="c4c6f-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="c4c6f-127">安裝 Office 更新</span><span class="sxs-lookup"><span data-stu-id="c4c6f-127">Install Office updates</span></span>
    
- <span data-ttu-id="c4c6f-128">執行 Office 線上修復</span><span class="sxs-lookup"><span data-stu-id="c4c6f-128">Perform an Online repair of Office</span></span>
    

