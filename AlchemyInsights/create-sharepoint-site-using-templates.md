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
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753698"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="a3b27-102">建立 SharePoint 網站使用範本</span><span class="sxs-lookup"><span data-stu-id="a3b27-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="a3b27-103">SharePoint 網站範本是預先的定義專為特定的業務需求。</span><span class="sxs-lookup"><span data-stu-id="a3b27-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="a3b27-104">如需詳細資訊，請參閱[使用範本來建立不同類型的 SharePoint 網站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。</span><span class="sxs-lookup"><span data-stu-id="a3b27-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="a3b27-105">以下是一些常見的問題/解決方案有關儲存網站或清單作為範本，在 Sharepoint Online 中。</span><span class="sxs-lookup"><span data-stu-id="a3b27-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="a3b27-106">**儲存網站/清單範本] 按鈕不提供或遺失**</span><span class="sxs-lookup"><span data-stu-id="a3b27-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="a3b27-107">系統管理員就必須允許自訂指令碼來啟用範本的功能。</span><span class="sxs-lookup"><span data-stu-id="a3b27-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="a3b27-108">如需詳細步驟，範例和考量請參閱</span><span class="sxs-lookup"><span data-stu-id="a3b27-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="a3b27-109">允許或防止自訂指令碼</span><span class="sxs-lookup"><span data-stu-id="a3b27-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="a3b27-110">另存網站為範本] 命令不支援，及使用 SharePoint Server 發佈基礎結構的網站上可能會造成問題。</span><span class="sxs-lookup"><span data-stu-id="a3b27-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="a3b27-111">[網站] 範本無法建立或無法正常運作。</span><span class="sxs-lookup"><span data-stu-id="a3b27-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="a3b27-112">範本可能會遺失的[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)，並不會啟動。</span><span class="sxs-lookup"><span data-stu-id="a3b27-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="a3b27-113">如果找不到可在目前的網站集合中啟動的功能，您無法使用網站範本建立網站。</span><span class="sxs-lookup"><span data-stu-id="a3b27-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="a3b27-114">請查看是否任何清單或文件庫超過 5000 的項目[清單檢視的限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)為這可以封鎖架設的網站範本。</span><span class="sxs-lookup"><span data-stu-id="a3b27-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="a3b27-115">網站使用太多的資源並因此網站範本超過 50 MB 的限制。</span><span class="sxs-lookup"><span data-stu-id="a3b27-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="a3b27-116">有問題，顯示使用查閱欄的清單中的資料。</span><span class="sxs-lookup"><span data-stu-id="a3b27-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="a3b27-117">如需詳細資訊，請參閱[範本產生清單不會顯示來自 SharePoint Online 中正確的查閱清單的資料](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。</span><span class="sxs-lookup"><span data-stu-id="a3b27-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="a3b27-118">針對常見的問題與解決方案的詳細資訊，請檢查[建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。</span><span class="sxs-lookup"><span data-stu-id="a3b27-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



