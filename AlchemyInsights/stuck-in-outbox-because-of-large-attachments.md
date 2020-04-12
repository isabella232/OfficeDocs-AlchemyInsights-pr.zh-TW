---
title: 因大附件而滯留于寄件匣
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232621"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="6c37a-102">修正寄件匣中停滯的郵件</span><span class="sxs-lookup"><span data-stu-id="6c37a-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="6c37a-103">我們建議您從受影響電腦上的[Microsoft 支援及修復](https://diagnostics.office.com/#/)小幫手工具中，執行「[我已有問題傳送、接收或尋找電子郵件訊息](https://aka.ms/SaRA-OutlookSendReceive)」案例。</span><span class="sxs-lookup"><span data-stu-id="6c37a-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="6c37a-104">當郵件在您的 [寄件匣] 中停滯時，最可能的原因是大型附件或「連線時立即傳送」選項未啟用。</span><span class="sxs-lookup"><span data-stu-id="6c37a-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="6c37a-105">**移除大型附件**</span><span class="sxs-lookup"><span data-stu-id="6c37a-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="6c37a-106">按一下 [**傳送/接收** > **離線工作**]。</span><span class="sxs-lookup"><span data-stu-id="6c37a-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="6c37a-107">在功能窗格中，按一下 [**寄件匣**]。</span><span class="sxs-lookup"><span data-stu-id="6c37a-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="6c37a-108">在這裡，您可以：</span><span class="sxs-lookup"><span data-stu-id="6c37a-108">From here, you can:</span></span> 
    - <span data-ttu-id="6c37a-109">刪除郵件。</span><span class="sxs-lookup"><span data-stu-id="6c37a-109">Delete the message.</span></span> <span data-ttu-id="6c37a-110">只需選取它，然後按一下 [**刪除**]。</span><span class="sxs-lookup"><span data-stu-id="6c37a-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="6c37a-111">將郵件拖曳至 [**草稿] 資料夾**，按兩下以開啟郵件，然後刪除附件（按一下該附件，然後按一下 [**刪除**]）。</span><span class="sxs-lookup"><span data-stu-id="6c37a-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="6c37a-112">如果錯誤告訴您 Outlook 嘗試傳輸郵件，請關閉 Outlook。</span><span class="sxs-lookup"><span data-stu-id="6c37a-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="6c37a-113">可能需要幾分鐘的時間才能結束。</span><span class="sxs-lookup"><span data-stu-id="6c37a-113">It may take a few moments to exit.</span></span> <span data-ttu-id="6c37a-114">若 Outlook 未關閉，請按**Ctrl + Alt + Delete** ，然後按一下 [**開始任務管理員**]。</span><span class="sxs-lookup"><span data-stu-id="6c37a-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="6c37a-115">在 **[任務**管理器] 中，選取 [程式] 索引標籤，向下滾動至 [excel.exe]，然後按一下 [**結束**程式]。</span><span class="sxs-lookup"><span data-stu-id="6c37a-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="6c37a-116">Outlook 關閉後，請重新開機 Outlook，然後重複步驟2-3。</span><span class="sxs-lookup"><span data-stu-id="6c37a-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="6c37a-117">移除附件後，請按一下 [**傳送/接收** > **離線工作**] 以取消選取按鈕，並繼續線上工作。</span><span class="sxs-lookup"><span data-stu-id="6c37a-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="6c37a-118">當您按一下 [**傳送**]，但未連接時，郵件也會在 [寄件匣] 中停滯。</span><span class="sxs-lookup"><span data-stu-id="6c37a-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="6c37a-119">按一下 [**傳送/接收**]，然後查看 [**工作離線工作**] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="6c37a-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="6c37a-120">如果是藍色，表示您已中斷連線。</span><span class="sxs-lookup"><span data-stu-id="6c37a-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="6c37a-121">按一下以進行連線（按鈕變成白色），然後按一下 [**全部傳送**]。</span><span class="sxs-lookup"><span data-stu-id="6c37a-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="6c37a-122">**啟用連線時立即傳送**</span><span class="sxs-lookup"><span data-stu-id="6c37a-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="6c37a-123">在 [檔案] 索引標籤上，按一下 [選項]。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="6c37a-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="6c37a-124">按一下 [Outlook 選項] 對話方塊中的 [進階]。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="6c37a-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="6c37a-125">在 [傳送及接收] 區段中，按一下以啟用**連線時立即傳送**。</span><span class="sxs-lookup"><span data-stu-id="6c37a-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="6c37a-126">按一下 [確定]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="6c37a-126">Click **OK**.</span></span>
 
<span data-ttu-id="6c37a-127">如需完整的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="6c37a-127">For full details, see:</span></span>
- [<span data-ttu-id="6c37a-128">影片：傳送或刪除卡住的電子郵件</span><span class="sxs-lookup"><span data-stu-id="6c37a-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- <span data-ttu-id="6c37a-129">[除非您在 Outlook 中手動啟動傳送/接收作業，否則電子郵件會保留在 [寄件匣] 資料夾中。](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span><span class="sxs-lookup"><span data-stu-id="6c37a-129">[Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span></span>
