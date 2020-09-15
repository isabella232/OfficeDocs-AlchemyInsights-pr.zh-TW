---
title: 將外部使用者新增至通訊群組
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663504"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="01c4d-102">將外部使用者新增至通訊群組</span><span class="sxs-lookup"><span data-stu-id="01c4d-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="01c4d-103">將外部連絡人新增至通訊群組 (DG) 分兩個步驟的程式：</span><span class="sxs-lookup"><span data-stu-id="01c4d-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="01c4d-104">為外部使用者建立郵件連絡人：</span><span class="sxs-lookup"><span data-stu-id="01c4d-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="01c4d-105">在系統管理中心中，移至 [**使用者**  >  [連絡人](https://admin.microsoft.com/adminportal/home#/Contact)] 頁面。</span><span class="sxs-lookup"><span data-stu-id="01c4d-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="01c4d-106">選取 [ **新增連絡人**]。</span><span class="sxs-lookup"><span data-stu-id="01c4d-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="01c4d-107">輸入您的連絡人資訊，然後選取 [ **新增**]。</span><span class="sxs-lookup"><span data-stu-id="01c4d-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="01c4d-108">將郵件連絡人新增至您的 DG:</span><span class="sxs-lookup"><span data-stu-id="01c4d-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="01c4d-109">在系統管理中心中，移至 [**群組**  >  [群組](https://admin.microsoft.com/adminportal/home#/groups)] 頁面。</span><span class="sxs-lookup"><span data-stu-id="01c4d-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="01c4d-110">尋找您要新增外部使用者的 DG，然後選取該 DG 以開啟 [編輯] 對話方塊。</span><span class="sxs-lookup"><span data-stu-id="01c4d-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="01c4d-111">在 [ **成員** ] 索引標籤上，選取 [ **全部查看] 和 [管理成員**]。</span><span class="sxs-lookup"><span data-stu-id="01c4d-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="01c4d-112">選取 [新增成員]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="01c4d-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="01c4d-113">選取您在上一個步驟中建立的郵件連絡人，然後選取 [ **儲存**]。</span><span class="sxs-lookup"><span data-stu-id="01c4d-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="01c4d-114">遵循這些步驟之後，您的外部使用者無法將電子郵件傳送至 DG，或是未接收到該 DG 的電子郵件，可能是該 DG 已標示為只允許來自內部使用者的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="01c4d-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="01c4d-115">您可以檢查此設定，並在 [這裡](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)遵循下列指示加以修正。</span><span class="sxs-lookup"><span data-stu-id="01c4d-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="01c4d-116">**附注：** 如果您的群組類型為 "Microsoft 365 group" 而非「通訊群組」，這些指示將不適用。</span><span class="sxs-lookup"><span data-stu-id="01c4d-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="01c4d-117">如果是這種情況，您可以從 Outlook 將外部使用者直接新增至群組。</span><span class="sxs-lookup"><span data-stu-id="01c4d-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="01c4d-118">有關 Microsoft 365 群組來賓的詳細資訊，以及新增外部來賓的指示，請參閱 [本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)。</span><span class="sxs-lookup"><span data-stu-id="01c4d-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  