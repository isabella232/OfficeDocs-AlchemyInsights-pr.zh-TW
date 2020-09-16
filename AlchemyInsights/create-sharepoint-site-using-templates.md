---
title: 在 SharePoint Online 中建立網站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732205"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="96108-102">使用範本建立 SharePoint 網站</span><span class="sxs-lookup"><span data-stu-id="96108-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="96108-103">新式通訊或小組網站不支援將網站儲存為範本的功能。</span><span class="sxs-lookup"><span data-stu-id="96108-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="96108-104">如需使用範本的詳細資訊 [，請參閱儲存、下載和上傳 SharePoint 網站為範本](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)。</span><span class="sxs-lookup"><span data-stu-id="96108-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="96108-105">以下是一些有關在 Sharepoint Online 中將網站或清單儲存為範本的常見問題/解決方案。</span><span class="sxs-lookup"><span data-stu-id="96108-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="96108-106">**無法使用或遺漏 [儲存網站/清單範本] 按鈕**</span><span class="sxs-lookup"><span data-stu-id="96108-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="96108-107">系統管理員必須允許自訂腳本啟用範本功能。</span><span class="sxs-lookup"><span data-stu-id="96108-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="96108-108">如需詳細步驟，請參閱</span><span class="sxs-lookup"><span data-stu-id="96108-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="96108-109">允許或防止自訂指令碼</span><span class="sxs-lookup"><span data-stu-id="96108-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="96108-110">[另存網站為範本] 命令不受支援，而且可能會導致使用 SharePoint 伺服器發佈基礎結構之網站的問題。</span><span class="sxs-lookup"><span data-stu-id="96108-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="96108-111">**無法建立或無法正常運作的網站範本**</span><span class="sxs-lookup"><span data-stu-id="96108-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="96108-112">範本可能遺漏了某 [項功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ，且無法啟動。</span><span class="sxs-lookup"><span data-stu-id="96108-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="96108-113">如果無法在目前的網站集合中啟動該功能，您就無法使用網站範本來建立網站。</span><span class="sxs-lookup"><span data-stu-id="96108-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="96108-114">檢查是否有任何清單或文件庫超出5000個專案的 [清單查看限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ，因為這會封鎖網站範本的建立。</span><span class="sxs-lookup"><span data-stu-id="96108-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="96108-115">網站可能使用太多資源，因此網站範本超過 50 MB 的限制。</span><span class="sxs-lookup"><span data-stu-id="96108-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="96108-116">使用查閱欄的清單顯示資料時出現問題。</span><span class="sxs-lookup"><span data-stu-id="96108-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="96108-117">如需詳細資訊，請參閱 [範本產生的清單，在 SharePoint Online 中不會顯示正確查閱清單中的資料](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。</span><span class="sxs-lookup"><span data-stu-id="96108-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="96108-118">如需有關常見問題和解決方案的詳細資訊，請參閱 [建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。</span><span class="sxs-lookup"><span data-stu-id="96108-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



