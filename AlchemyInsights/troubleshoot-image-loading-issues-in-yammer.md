---
title: 疑難排解 Yammer 中的圖像載入問題
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
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690234"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="5575c-102">疑難排解 Yammer 中的圖像載入問題</span><span class="sxs-lookup"><span data-stu-id="5575c-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="5575c-103">當您在 Yammer 中有相片和檔案預覽的問題時，請透過檢查是否所有使用者無論是否使用行動裝置都有此問題，以及上傳附件時是否可重複使用，以進行移難排解。</span><span class="sxs-lookup"><span data-stu-id="5575c-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="5575c-104">**個人檔案相片問題**</span><span class="sxs-lookup"><span data-stu-id="5575c-104">**Profile photo issues**</span></span>  

<span data-ttu-id="5575c-105">如果使用者透過 Microsoft 365 登入 Yammer，他們必須變更自己的個人檔案，包括個人檔案相片。</span><span class="sxs-lookup"><span data-stu-id="5575c-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="5575c-106">如果使用者不允許您變更個人檔案，系統管理員可以為使用者進行更新。</span><span class="sxs-lookup"><span data-stu-id="5575c-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="5575c-107">如需詳細資訊，請參閱[在 Office Delve 中檢視和編輯您的個人檔案](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)。</span><span class="sxs-lookup"><span data-stu-id="5575c-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="5575c-108">如需個人檔案編輯的相關資訊，包括個人檔案相片，請參閱 [變更我的 Yammer 個人檔案和設定](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)。</span><span class="sxs-lookup"><span data-stu-id="5575c-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="5575c-109">更新後的個人檔案相片與個人檔案屬性的同步方式不同。</span><span class="sxs-lookup"><span data-stu-id="5575c-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="5575c-110">使用者必須登入才能開始同步處理個人檔案相片。</span><span class="sxs-lookup"><span data-stu-id="5575c-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="5575c-111">如需詳細資訊，請參閱 [是否使用者個人檔案圖片會從 Office 365 更新至 Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)。</span><span class="sxs-lookup"><span data-stu-id="5575c-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="5575c-112">如需 Yammer 使用者生命週期的相關資訊，請參閱 [從 Office 365 管理 Yammer 使用者的整體生命週期。](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)</span><span class="sxs-lookup"><span data-stu-id="5575c-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="5575c-113">如需有關如何在 Microsoft 365 中執行個人檔案相片同步處理的詳細資訊，請參閱 [Microsoft 365 中的個人檔案同步處理相關資訊。](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)</span><span class="sxs-lookup"><span data-stu-id="5575c-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="5575c-114">**文件預覽和影像縮圖問題**</span><span class="sxs-lookup"><span data-stu-id="5575c-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="5575c-115">當檔案或影像張貼至 Yammer 時，可能不會顯示出預覽：</span><span class="sxs-lookup"><span data-stu-id="5575c-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="5575c-116">檔案已經損毀，無法處理。</span><span class="sxs-lookup"><span data-stu-id="5575c-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="5575c-117">檔案最近尚未上傳至 SharePoint Online，或是 Yammer 因其他原因而元數據無效。</span><span class="sxs-lookup"><span data-stu-id="5575c-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="5575c-118">系統會封鎖載入預覽影像所需的 URL。</span><span class="sxs-lookup"><span data-stu-id="5575c-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="5575c-119">張貼前，使用者已移除檔案預覽。</span><span class="sxs-lookup"><span data-stu-id="5575c-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="5575c-120">服務問題造成無法產生預覽。</span><span class="sxs-lookup"><span data-stu-id="5575c-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="5575c-121">**附注** 連結和檔案上傳的預覽可能會有所不同。</span><span class="sxs-lookup"><span data-stu-id="5575c-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="5575c-122">連結至網路上的檔案，或要求額外驗證的連結可能無法正確顯示。</span><span class="sxs-lookup"><span data-stu-id="5575c-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="5575c-123">如需詳細資訊，請參閱 [將檔案或影像附加至 Yammer 郵件](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)。</span><span class="sxs-lookup"><span data-stu-id="5575c-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 