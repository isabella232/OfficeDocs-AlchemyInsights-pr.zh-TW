---
title: 因為大型附件一直停留在寄件匣
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441297"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="71f37-102">修正卡在寄件匣中的郵件</span><span class="sxs-lookup"><span data-stu-id="71f37-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="71f37-103">我們建議您開始執行從[Microsoft 支援及修復小幫手](https://diagnostics.office.com/#/)工具的 [ [「 我所遇到問題傳送、 接收或找出電子郵件 」](https://aka.ms/SaRA-OutlookSendReceive)的案例。</span><span class="sxs-lookup"><span data-stu-id="71f37-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="71f37-104">當郵件卡住寄件匣中時，最可能的原因如下：</span><span class="sxs-lookup"><span data-stu-id="71f37-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="71f37-105">大型附件。</span><span class="sxs-lookup"><span data-stu-id="71f37-105">Large attachments.</span></span>
- <span data-ttu-id="71f37-106">未啟用 [**連線時，立即傳送**] 選項。</span><span class="sxs-lookup"><span data-stu-id="71f37-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="71f37-107">若要移除大型附件：</span><span class="sxs-lookup"><span data-stu-id="71f37-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="71f37-108">在 Outlook 中，選取 [**傳送 / 接收** > **離線工作**。</span><span class="sxs-lookup"><span data-stu-id="71f37-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="71f37-109">在 [功能窗格中，選取 [**寄件匣**]。</span><span class="sxs-lookup"><span data-stu-id="71f37-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="71f37-110">從這裡開始，您可以：</span><span class="sxs-lookup"><span data-stu-id="71f37-110">From here, you can:</span></span> 
    - <span data-ttu-id="71f37-111">刪除郵件 （選取它，然後選取 [**刪除**）。</span><span class="sxs-lookup"><span data-stu-id="71f37-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="71f37-112">將郵件拖曳至 [草稿] 資料夾，連按兩下以開啟它，並移除附件選取它，然後選取 [**刪除**）。</span><span class="sxs-lookup"><span data-stu-id="71f37-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="71f37-113">如果您收到錯誤，指出 Outlook 正嘗試傳送郵件時，關閉 Outlook。</span><span class="sxs-lookup"><span data-stu-id="71f37-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="71f37-114">可能需要一些時間才能結束。</span><span class="sxs-lookup"><span data-stu-id="71f37-114">It may take a few moments to exit.</span></span> <span data-ttu-id="71f37-115">如果 Outlook 不會關閉，請按 Ctrl + Alt + Delete 鍵，然後選取 [**啟動工作管理員]**。</span><span class="sxs-lookup"><span data-stu-id="71f37-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="71f37-116">在 [工作管理員] 中，選取 [**程序**] 索引標籤，捲動至 [outlook.exe，然後選取 [**結束處理程序**。</span><span class="sxs-lookup"><span data-stu-id="71f37-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="71f37-117">Outlook 關閉之後，重新啟動它，然後重複步驟 2 和 3。</span><span class="sxs-lookup"><span data-stu-id="71f37-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="71f37-118">移除附件之後，按一下 [**傳送 / 接收** > **離線工作**，繼續線上工作。</span><span class="sxs-lookup"><span data-stu-id="71f37-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="71f37-119">郵件也不知道寄件匣中按一下 [**傳送**]，但您無法連線時。</span><span class="sxs-lookup"><span data-stu-id="71f37-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="71f37-120">按一下 [**傳送 / 接收**，然後查看 [**離線工作**] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="71f37-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="71f37-121">如果顯示藍色，您要中斷連線。</span><span class="sxs-lookup"><span data-stu-id="71f37-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="71f37-122">選取連線 （白色的按鈕開啟），並按一下 **[全部傳送**它。</span><span class="sxs-lookup"><span data-stu-id="71f37-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="71f37-123">若要啟用**連線時，立即傳送**：</span><span class="sxs-lookup"><span data-stu-id="71f37-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="71f37-124">選取**檔案** > **選項** >  **進階**。</span><span class="sxs-lookup"><span data-stu-id="71f37-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="71f37-125">在**傳送及接收**] 區段中，選取 [**連線時，立即傳送**，然後再選擇 [**確定]**。</span><span class="sxs-lookup"><span data-stu-id="71f37-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="71f37-126">完整詳細資料，請參閱：</span><span class="sxs-lookup"><span data-stu-id="71f37-126">For full details see:</span></span>
- <span data-ttu-id="71f37-127">[影片： 傳送] 或 [刪除的停滯的電子郵件](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec)</span><span class="sxs-lookup"><span data-stu-id="71f37-127">[Video: Send or delete a stuck email](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec)</span></span> 
- <span data-ttu-id="71f37-128">[電子郵件會停留在 [寄件匣] 資料夾，直到您手動啟動 Outlook 傳送/接收作業](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span><span class="sxs-lookup"><span data-stu-id="71f37-128">[Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)</span></span>
