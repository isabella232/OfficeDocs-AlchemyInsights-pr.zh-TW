---
title: 在 Yammer 中發布開啟的或下載的檔案
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695640"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="a8ec8-102">在 Yammer 中發布開啟的或下載的檔案</span><span class="sxs-lookup"><span data-stu-id="a8ec8-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="a8ec8-103">傳統的 Yammer 支援多種上傳檔案到郵件和群組的選項。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="a8ec8-104">根據網路設定，檔案預設為儲存在 SharePoint 中。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="a8ec8-105">新版 Yammer 中的檔案選擇器尚未支援傳統 Yammer 中提供的所有選項。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="a8ec8-106">未來的更新將新增其他功能。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-106">A future update will add additional features.</span></span> <span data-ttu-id="a8ec8-107">如需詳細資訊，請參閱 [將檔案或影像附加至 Yammer 對話文章中](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="a8ec8-108">**無法開啟或下載檔案**</span><span class="sxs-lookup"><span data-stu-id="a8ec8-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="a8ec8-109">檔案可能會上傳至 Yammer，但也會連結至 SharePoint Online 中的檔案。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="a8ec8-110">若要進行疑難排解，您必須先決定檔案的位置。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="a8ec8-111">如果檔案已下載到 Yammer，則會有 \*.yammer.com 的URL。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="a8ec8-112">確保要求的 URL 和 IP 位置未被封鎖。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="a8ec8-113">如需詳細資訊，請參閱部落格文章 [不推薦在 Ymmer 上使用硬編碼 IP 位址](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="a8ec8-114">請查看是否也是全域系統管理人的使用者可以下載檔案。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="a8ec8-115">如果檔案為私人檔案，您可能需要使用 [私人內容模式]。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="a8ec8-116">如需詳細資訊，請參閱 [監視 Yammer 中的私人內容](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="a8ec8-117">**Yammer 網路層級來賓和 SharePoint Online 中的檔案**</span><span class="sxs-lookup"><span data-stu-id="a8ec8-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="a8ec8-118">[Yammer 中的網路層級來賓](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) 不使用 Azure AD B2B 且為 Yammer 服務的內部使用者，因此他們無法存取儲存在 SharePoint 中的 Yammer 檔案。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="a8ec8-119">建立可使用該身分識別在 SharePoint Online 中存取文件庫的外部 AAD B2B 使用者。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="a8ec8-120">如需 Yammer 中未來 Azure AD B2B 來賓支援的相關資訊，請參閱 [在 Yammer 預覽中的企業對企業（B2B）來賓支援-客戶條款與常見問題](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)。</span><span class="sxs-lookup"><span data-stu-id="a8ec8-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>