---
title: 在 SharePoint Online 中建立網站
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199264"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c3311-102">使用範本建立 SharePoint 網站</span><span class="sxs-lookup"><span data-stu-id="c3311-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c3311-103">SharePoint 網站範本是專為特定業務需求而設計的預置定義。</span><span class="sxs-lookup"><span data-stu-id="c3311-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="c3311-104">如需詳細資訊, 請參閱[使用範本建立不同類型的 SharePoint 網站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。</span><span class="sxs-lookup"><span data-stu-id="c3311-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="c3311-105">以下是有關在 Sharepoint Online 中將網站或清單儲存為範本的一些常見問題/解決方案。</span><span class="sxs-lookup"><span data-stu-id="c3311-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c3311-106">**[儲存網站/清單範本] 按鈕無法使用或遺失**</span><span class="sxs-lookup"><span data-stu-id="c3311-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c3311-107">系統管理員必須允許自訂腳本啟用範本功能。</span><span class="sxs-lookup"><span data-stu-id="c3311-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c3311-108">如需詳細步驟, 請參閱</span><span class="sxs-lookup"><span data-stu-id="c3311-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c3311-109">允許或防止自訂指令碼</span><span class="sxs-lookup"><span data-stu-id="c3311-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c3311-110">不支援 [另存網站為範本] 命令, 而且可能會在使用 SharePoint Server 發佈基礎結構的網站上造成問題。</span><span class="sxs-lookup"><span data-stu-id="c3311-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c3311-111">**無法建立或無法正常運作網站範本**</span><span class="sxs-lookup"><span data-stu-id="c3311-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c3311-112">範本可能遺失[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)且不會啟動。</span><span class="sxs-lookup"><span data-stu-id="c3311-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c3311-113">如果無法在目前的網站集合中啟用此功能, 您就無法使用網站範本來建立網站。</span><span class="sxs-lookup"><span data-stu-id="c3311-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c3311-114">檢查是否有任何清單或文件庫超出5000個專案的[清單查看限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), 因為這會封鎖網站範本的建立。</span><span class="sxs-lookup"><span data-stu-id="c3311-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c3311-115">網站可能使用太多資源, 因此網站範本超過 50 MB 的限制。</span><span class="sxs-lookup"><span data-stu-id="c3311-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c3311-116">顯示使用查閱欄之清單中的資料時發生問題。</span><span class="sxs-lookup"><span data-stu-id="c3311-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c3311-117">如需詳細資訊, 請參閱[範本產生的清單不會在 SharePoint Online 中顯示正確查閱清單中的資料](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。</span><span class="sxs-lookup"><span data-stu-id="c3311-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="c3311-118">如需常見問題和解決方案的詳細資訊, 請參閱[Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。</span><span class="sxs-lookup"><span data-stu-id="c3311-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



