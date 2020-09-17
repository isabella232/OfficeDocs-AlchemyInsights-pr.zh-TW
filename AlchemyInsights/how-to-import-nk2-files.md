---
title: nk2-import-import-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780050"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="3c643-102">如何匯入 nk2 檔案</span><span class="sxs-lookup"><span data-stu-id="3c643-102">How to import .nk2 files</span></span> 

<span data-ttu-id="3c643-103">當您第一次啟動 Microsoft Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365 時，您的昵稱快取快取 (儲存在預設郵件存放區 *中的 nk2*檔案中) 會匯入到隱藏的郵件中。</span><span class="sxs-lookup"><span data-stu-id="3c643-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="3c643-104">若要將 nk2 檔案匯入 Outlook 2013、Outlook 2016、Outlook 2019 或 Outlook for Microsoft 365，請確定 nk2 檔案位於下列資料夾中：%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="3c643-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="3c643-105">**附注**： nk2 檔案必須與您目前的 outlook 2013 或 outlook 2016 設定檔同名。</span><span class="sxs-lookup"><span data-stu-id="3c643-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="3c643-106">設定檔名稱預設為 "Outlook"。</span><span class="sxs-lookup"><span data-stu-id="3c643-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="3c643-107">若要檢查設定檔名稱，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="3c643-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="3c643-108">按一下 **[開始]**，然後按一下 **[控制台]**。</span><span class="sxs-lookup"><span data-stu-id="3c643-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="3c643-109">連按兩下 [ **郵件**]。</span><span class="sxs-lookup"><span data-stu-id="3c643-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="3c643-110">在 [郵件設定] 對話方塊中，選取 [ **顯示設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="3c643-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="3c643-111">選取 [**啟動**  >  **執行**]。</span><span class="sxs-lookup"><span data-stu-id="3c643-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="3c643-112">在 [ **開啟** ] 方塊中，輸入 *outlook.exe/importnk2*]，然後選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="3c643-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="3c643-113">當您匯入 nk2 檔之後，檔案的內容會合並至儲存在信箱中的現有昵稱快取。</span><span class="sxs-lookup"><span data-stu-id="3c643-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="3c643-114">**附注**：下一次啟動 outlook 2013、outlook 2016、outlook 2019 或 Outlook for Microsoft 365 時，會以 .old 副檔名重新命名 nk2 檔案。</span><span class="sxs-lookup"><span data-stu-id="3c643-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="3c643-115">如果想要重新匯入 nk2 檔，請先移除 .old 副檔名。</span><span class="sxs-lookup"><span data-stu-id="3c643-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="3c643-116">如需詳細資訊，請參閱匯 [入或複製自動完成清單到另一部電腦](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)。</span><span class="sxs-lookup"><span data-stu-id="3c643-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>