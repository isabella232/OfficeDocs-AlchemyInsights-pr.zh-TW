---
title: 將外部使用者新增至通訊群組
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737864"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="efd63-102">將外部使用者新增至通訊群組</span><span class="sxs-lookup"><span data-stu-id="efd63-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="efd63-103">新增外部連絡人至通訊群組 (DG) 是一個兩步驟程序：</span><span class="sxs-lookup"><span data-stu-id="efd63-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="efd63-104">建立郵件連絡人的外部使用者：</span><span class="sxs-lookup"><span data-stu-id="efd63-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="efd63-105">在系統管理中心，移至 [**使用者** > [連絡人](https://admin.microsoft.com/adminportal/home#/Contact)] 頁面。</span><span class="sxs-lookup"><span data-stu-id="efd63-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="efd63-106">選取 [**新增連絡人**。</span><span class="sxs-lookup"><span data-stu-id="efd63-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="efd63-107">輸入您的連絡人資訊，然後選取 [**新增]**。</span><span class="sxs-lookup"><span data-stu-id="efd63-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="efd63-108">將郵件連絡人新增至您 DG:</span><span class="sxs-lookup"><span data-stu-id="efd63-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="efd63-109">在系統管理中心，移至 [**群組** > [群組](https://admin.microsoft.com/adminportal/home#/groups)] 頁面。</span><span class="sxs-lookup"><span data-stu-id="efd63-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="efd63-110">尋找您想要將外部使用者加入，的 DG，然後選取 [以開啟 [編輯] 對話方塊。</span><span class="sxs-lookup"><span data-stu-id="efd63-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="efd63-111">在 [**成員**] 索引標籤中，選取 [**檢視所有及管理成員**。</span><span class="sxs-lookup"><span data-stu-id="efd63-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="efd63-112">選取 [**新增成員**。</span><span class="sxs-lookup"><span data-stu-id="efd63-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="efd63-113">選取您在前一個步驟中，建立郵件連絡人，然後選取 [**儲存**。</span><span class="sxs-lookup"><span data-stu-id="efd63-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="efd63-114">如果執行這些步驟之後您的外部使用者無法傳送電子郵件給 DG，或未收到電子郵件從它，它可能是 DG 被標記為僅允許來自內部使用者的 [電子郵件。</span><span class="sxs-lookup"><span data-stu-id="efd63-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="efd63-115">您可以檢查此組態並修正下列指示[以下](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="efd63-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="efd63-116">**附註：** 這些指示不適用，如果您的群組類型是 「 Office 365 群組 」 而不是 「 通訊群組 」。</span><span class="sxs-lookup"><span data-stu-id="efd63-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="efd63-117">如果是這種情況，您可以直接對群組新增外部使用者，從 Outlook 項目。</span><span class="sxs-lookup"><span data-stu-id="efd63-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="efd63-118">在 Office 365 群組來賓的詳細的資訊以及指示新增外部訪客可以在[本文](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)中找到。</span><span class="sxs-lookup"><span data-stu-id="efd63-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  