---
title: 將網站或清單另存為範本
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727522"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="4e75d-102">將網站或清單另存為範本</span><span class="sxs-lookup"><span data-stu-id="4e75d-102">Save site or list as a template</span></span>

<span data-ttu-id="4e75d-103">SharePoint 網站範本是針對特定商務需求所設計的預置定義。</span><span class="sxs-lookup"><span data-stu-id="4e75d-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="4e75d-104">如需詳細資訊，請參閱 [使用範本建立不同類型的 SharePoint 網站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。</span><span class="sxs-lookup"><span data-stu-id="4e75d-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="4e75d-105">以下是一些常見的問題/解決方案，有關將網站或清單儲存為 SharePoint 線上中的範本。</span><span class="sxs-lookup"><span data-stu-id="4e75d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="4e75d-106">**無法使用或遺漏 [儲存網站/清單範本] 按鈕**。</span><span class="sxs-lookup"><span data-stu-id="4e75d-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="4e75d-107">系統管理員必須允許自訂腳本啟用範本功能。</span><span class="sxs-lookup"><span data-stu-id="4e75d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="4e75d-108">如需詳細步驟，請參閱 [Allow 或預防自訂腳本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="4e75d-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="4e75d-109">[另存網站為範本] 命令不受支援，而且可能會導致使用 SharePoint 伺服器發佈基礎結構之網站的問題。</span><span class="sxs-lookup"><span data-stu-id="4e75d-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="4e75d-110">**無法建立或無法正常運作的網站範本**</span><span class="sxs-lookup"><span data-stu-id="4e75d-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="4e75d-111">範本可能遺漏了某 [項功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ，且無法啟動。</span><span class="sxs-lookup"><span data-stu-id="4e75d-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="4e75d-112">如果無法在目前的網站集合中啟動該功能，您就無法使用網站範本來建立網站。</span><span class="sxs-lookup"><span data-stu-id="4e75d-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="4e75d-113">檢查是否有任何清單或文件庫超出5000個專案的 [清單查看限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ，因為這會封鎖網站範本的建立。</span><span class="sxs-lookup"><span data-stu-id="4e75d-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="4e75d-114">網站可能使用太多資源，因此網站範本超過 50 mb (MB) 限制。</span><span class="sxs-lookup"><span data-stu-id="4e75d-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="4e75d-115">使用查閱欄的清單顯示資料時出現問題。</span><span class="sxs-lookup"><span data-stu-id="4e75d-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="4e75d-116">如需詳細資訊，請參閱 [範本產生的清單，在 SharePoint Online 中不會顯示正確查閱清單中的資料](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。</span><span class="sxs-lookup"><span data-stu-id="4e75d-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="4e75d-117">如需有關常見問題和解決方案的詳細資訊，請參閱 [建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。</span><span class="sxs-lookup"><span data-stu-id="4e75d-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

