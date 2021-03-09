---
title: 透過提供網路郵件識別碼提交電子郵件訊息
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552290"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="99367-102">透過提供網路郵件識別碼提交電子郵件訊息</span><span class="sxs-lookup"><span data-stu-id="99367-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="99367-103">在 **新的提交** 快顯視窗中，選取 [ **電子郵件** 和 **網路消息識別碼**]。</span><span class="sxs-lookup"><span data-stu-id="99367-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="99367-104">請遵循下列步驟，在 Outlook 中尋找電子郵件的郵件識別碼：</span><span class="sxs-lookup"><span data-stu-id="99367-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="99367-105">按兩下電子郵件以開啟它。</span><span class="sxs-lookup"><span data-stu-id="99367-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="99367-106">選取 [**檔**  >  **屬性**]。</span><span class="sxs-lookup"><span data-stu-id="99367-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="99367-107">開啟 [記事本] 或空白的 Word 檔，然後複製並貼上 [ **Internet 標頭** ] 方塊中找到的內容，以取得更好的知名度。</span><span class="sxs-lookup"><span data-stu-id="99367-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="99367-108">找出 **X-MS-Exchange-Organization-網路 Message-Id** ] 欄位。</span><span class="sxs-lookup"><span data-stu-id="99367-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="99367-109">在 **：** 之後的值是您提交所需的識別碼。</span><span class="sxs-lookup"><span data-stu-id="99367-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="99367-110">在 **[** 收件者] 底下的 [垃圾郵件] 資料夾中進入此電子郵件的所有收件者，請選擇 [ **全選**]。</span><span class="sxs-lookup"><span data-stu-id="99367-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="99367-111">如果不是，請只選取報告問題的使用者。</span><span class="sxs-lookup"><span data-stu-id="99367-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="99367-112">在 **提交的原因** 下，如果您選取 [ **應該已封鎖**]，請指定是否應該封鎖郵件為 **垃圾郵件**、 **網路釣魚** 或 **惡意** 代碼，然後選取 [ **提交**]。</span><span class="sxs-lookup"><span data-stu-id="99367-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="99367-113">若要深入瞭解，請參閱 how [to 提交可疑的垃圾郵件、網路釣魚、URLs 及檔案給 Microsoft 進行掃描](https://go.microsoft.com/fwlink/?linkid=2101479)。</span><span class="sxs-lookup"><span data-stu-id="99367-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
