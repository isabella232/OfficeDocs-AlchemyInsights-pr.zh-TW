---
title: 唯讀檔案
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745565"
---
# <a name="file-open-read-only"></a><span data-ttu-id="8fc9e-102">唯讀檔案</span><span class="sxs-lookup"><span data-stu-id="8fc9e-102">File open read-only</span></span>

<span data-ttu-id="8fc9e-103">您可能會發現，當您開啟檔案時，這些檔案會以唯讀方式開啟。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="8fc9e-104">在某些情況下，這是為了增加安全性，例如當您從網際網路開啟檔案時，以及其他時間，這可能是因為可變更的設定。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="8fc9e-105">以下是一些檔案開啟唯讀的情況，以及您可以採取的一些步驟來變更該檔案。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="8fc9e-106">**我的防病毒已導致其以唯讀方式開啟**</span><span class="sxs-lookup"><span data-stu-id="8fc9e-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="8fc9e-107">某些防毒程式可能會以唯讀方式開啟，以保護可能不安全的檔案。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="8fc9e-108">您可能需要與您的防病毒提供者核實，以瞭解如何調整這些設定。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="8fc9e-109">例如，BitDefender 在這裡新增應用程式排除的內容： [如何在 BitDefender 的 [控制中心] 中新增應用程式或進程排除](https://aka.ms/AA6098i)。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="8fc9e-110">**檔案屬性是否設為唯讀？**</span><span class="sxs-lookup"><span data-stu-id="8fc9e-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="8fc9e-111">您可以在檔上按一下滑鼠右鍵，然後選擇 [內容]，檢查檔案屬性。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="8fc9e-112">如果已選取 [唯讀] 屬性，您可以取消選取它，然後按一下 [確定]。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="8fc9e-113">**內容位於受保護的檢視中**</span><span class="sxs-lookup"><span data-stu-id="8fc9e-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="8fc9e-114">來自網際網路的檔案與其他可能不安全的位置，可能包含病毒、蠕蟲或其他類型的惡意程式碼，可能會損害您的電腦。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="8fc9e-115">這通常也是您下載的電子郵件附件或檔案的案例。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="8fc9e-116">為了協助保護您的電腦，來自這些可能不安全之位置的檔案會在受保護的檢視中開啟。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="8fc9e-117">使用受保護的檢視，您可以讀取檔案並查看其內容，同時降低風險。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="8fc9e-118">如需受保護的檢視以及如何變更設定的詳細資訊，請參閱本文： [什麼是受保護的檢視？](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="8fc9e-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="8fc9e-119">**是否 OneDrive 完整？**</span><span class="sxs-lookup"><span data-stu-id="8fc9e-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="8fc9e-120">如果檔案儲存在 OneDrive，而您的 OneDrive 儲存空間已滿，您將無法儲存檔，除非您已在所分配的空間下。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="8fc9e-121">您可以按一下 [通知中心] 中的 [OneDrive] 圖示，然後選擇 [管理儲存]， [https://onedrive.live.com](https://onedrive.live.com) 再登入，並記下螢幕左下方的使用空間量，以查看 OneDrive 的可用空間。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="8fc9e-122">**Office 是否已啟用？**</span><span class="sxs-lookup"><span data-stu-id="8fc9e-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="8fc9e-123">如果未啟用 Office，或訂閱已過期，您可以處於唯讀的「精簡功能」模式。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="8fc9e-124">如需如何啟動 Office 的資訊，請參閱： [office 中的「未經許可的產品和啟用錯誤](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)」。</span><span class="sxs-lookup"><span data-stu-id="8fc9e-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="8fc9e-125">**如果其他所有失敗**</span><span class="sxs-lookup"><span data-stu-id="8fc9e-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="8fc9e-126">嘗試重新開機電腦</span><span class="sxs-lookup"><span data-stu-id="8fc9e-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="8fc9e-127">安裝 Office 更新</span><span class="sxs-lookup"><span data-stu-id="8fc9e-127">Install Office updates</span></span>
    
- <span data-ttu-id="8fc9e-128">執行 Office 的線上修復</span><span class="sxs-lookup"><span data-stu-id="8fc9e-128">Perform an Online repair of Office</span></span>
    

