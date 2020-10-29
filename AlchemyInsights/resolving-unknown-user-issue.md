---
title: 解決小組聊天中的未知使用者問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/28/2020
ms.locfileid: "48785571"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="60eac-102">解決小組聊天中的「未知使用者」問題</span><span class="sxs-lookup"><span data-stu-id="60eac-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="60eac-103">在此情況下，已移除的使用者會顯示為「未知使用者」。</span><span class="sxs-lookup"><span data-stu-id="60eac-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="60eac-104">這是 [已知問題](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown)。</span><span class="sxs-lookup"><span data-stu-id="60eac-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="60eac-105">如果您在「小組聊天」中持續看到使用者顯示為「未知使用者」，請嘗試並清除快取：</span><span class="sxs-lookup"><span data-stu-id="60eac-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="60eac-106">在工作列中，以滑鼠右鍵按一下小組圖示。</span><span class="sxs-lookup"><span data-stu-id="60eac-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="60eac-107">按一下  **[** 結束]。</span><span class="sxs-lookup"><span data-stu-id="60eac-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="60eac-108">在電腦上瀏覽至 %appdata%\Microsoft\teams\ 資料夾，刪除該目錄中的所有檔案。</span><span class="sxs-lookup"><span data-stu-id="60eac-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="60eac-109">您可以確認匿名使用者在會議廳中等待，以防止匿名使用者加入會議。</span><span class="sxs-lookup"><span data-stu-id="60eac-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="60eac-110">如需詳細資訊，請參閱 [變更小組會議的參與者設定](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)。</span><span class="sxs-lookup"><span data-stu-id="60eac-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
