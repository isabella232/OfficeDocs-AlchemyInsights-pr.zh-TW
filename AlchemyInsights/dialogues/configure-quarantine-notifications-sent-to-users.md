---
title: 設定傳送給使用者的隔離通知
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
- "9002531"
- "7375"
ms.openlocfilehash: 3e3e350f74b19420155c29cb282f065e7db6d4d7
ms.sourcegitcommit: 1f998ca586c90330fde515525432072f766d485b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50520564"
---
# <a name="configure-quarantine-notifications-sent-to-users"></a><span data-ttu-id="5ac92-102">設定傳送給使用者的隔離通知</span><span class="sxs-lookup"><span data-stu-id="5ac92-102">Configure quarantine notifications sent to users</span></span>

<span data-ttu-id="5ac92-103">若要將通知傳送給使用者，瞭解隔離的內容：</span><span class="sxs-lookup"><span data-stu-id="5ac92-103">To send notifications to your users about what's in quarantine:</span></span>

1. <span data-ttu-id="5ac92-104">在系統管理中心中，流覽至 [系統 **管理中心**] [  >  **Exchange**  >  **保護**  >  **垃圾郵件篩選**]。</span><span class="sxs-lookup"><span data-stu-id="5ac92-104">In the admin center, navigate to **admin centers** > **Exchange** > **Protection** > **spam filter**.</span></span>
2. <span data-ttu-id="5ac92-105">選取您要開啟通知的垃圾郵件篩選原則。</span><span class="sxs-lookup"><span data-stu-id="5ac92-105">Select the spam filter policy for which you want to turn on notifications.</span></span>
3. <span data-ttu-id="5ac92-106">在右窗格中，選擇 [ **設定使用者垃圾郵件通知** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="5ac92-106">In the right pane, choose the **Configure End-user spam notifications** link.</span></span>
4. <span data-ttu-id="5ac92-107">在 [下一個] 對話方塊中，選擇 [ **啟用使用者垃圾郵件通知**]。</span><span class="sxs-lookup"><span data-stu-id="5ac92-107">In the next dialog box, choose **Enable end-user spam notifications**.</span></span> <span data-ttu-id="5ac92-108">選擇啟用此原則的垃圾郵件通知。</span><span class="sxs-lookup"><span data-stu-id="5ac92-108">Choose to enable spam notifications for this policy.</span></span>
5. <span data-ttu-id="5ac92-109">在 [ **每 (天) 傳送使用者垃圾郵件通知**] 中，指定傳送使用者垃圾郵件通知的頻率。</span><span class="sxs-lookup"><span data-stu-id="5ac92-109">In **Send end-user spam notifications every (days)**, specify how often to send user spam notifications.</span></span> <span data-ttu-id="5ac92-110">預設值為 3 天。</span><span class="sxs-lookup"><span data-stu-id="5ac92-110">The default is 3 days.</span></span> <span data-ttu-id="5ac92-111">您可以指定 1 到 15 天之間的值。</span><span class="sxs-lookup"><span data-stu-id="5ac92-111">You can specify between 1 and 15 days.</span></span> <span data-ttu-id="5ac92-112">例如，如果您指定 7 天，則此通知將包含在過去 7 天內對象為該使用者，卻被當成垃圾郵件隔離的所有郵件的清單。</span><span class="sxs-lookup"><span data-stu-id="5ac92-112">If you specify 7 days, for example, the notification will include a list of all messages intended for that user within the past 7 days that were sent to the spam quarantine instead.</span></span>
6. <span data-ttu-id="5ac92-113">在 [ **通知語言** ] 中，選擇用來撰寫此原則之使用者垃圾郵件通知的語言。</span><span class="sxs-lookup"><span data-stu-id="5ac92-113">In **Notification language** choose the language in which to write user spam notifications for this policy.</span></span>
7. <span data-ttu-id="5ac92-114">選擇 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="5ac92-114">Choose **Save**.</span></span>
