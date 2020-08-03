---
title: 暫停排定的更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "46530585"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="49137-102">暫停排定的更新</span><span class="sxs-lookup"><span data-stu-id="49137-102">Pausing scheduled updates</span></span>

<span data-ttu-id="49137-103">發出 [暫停] 命令時，裝置在您下次登入 Intune 之前，不會處理命令。</span><span class="sxs-lookup"><span data-stu-id="49137-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="49137-104">因此，您的裝置可能：</span><span class="sxs-lookup"><span data-stu-id="49137-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="49137-105">在簽入前已安裝排定的更新。</span><span class="sxs-lookup"><span data-stu-id="49137-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="49137-106">在您發出 [暫停] 命令時已關閉電源。</span><span class="sxs-lookup"><span data-stu-id="49137-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="49137-107">在此情況下，當裝置電源開啟時，他們可能會在簽入前先下載並安裝排定的更新。</span><span class="sxs-lookup"><span data-stu-id="49137-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>