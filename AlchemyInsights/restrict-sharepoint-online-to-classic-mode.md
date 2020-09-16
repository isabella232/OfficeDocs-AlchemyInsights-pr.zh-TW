---
title: 將 SharePoint 線上限制為傳統模式
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751413"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="e1c99-102">將 SharePoint 線上限制為傳統模式</span><span class="sxs-lookup"><span data-stu-id="e1c99-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="e1c99-103">有些組織仍然需要傳統模式體驗。</span><span class="sxs-lookup"><span data-stu-id="e1c99-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="e1c99-104">雖然沒有任何計畫在細微層級移除傳統模式，但無法再將整個組織 (租使用者) 至傳統模式，以供清單和文件庫使用。</span><span class="sxs-lookup"><span data-stu-id="e1c99-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="e1c99-105">系統管理員可以使用下列方式，以傳統模式管理個別的清單和文件庫，其可在下列層級提供：</span><span class="sxs-lookup"><span data-stu-id="e1c99-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="e1c99-106">網站集合</span><span class="sxs-lookup"><span data-stu-id="e1c99-106">site collection</span></span>
- <span data-ttu-id="e1c99-107">網站</span><span class="sxs-lookup"><span data-stu-id="e1c99-107">site</span></span>
- <span data-ttu-id="e1c99-108">清單</span><span class="sxs-lookup"><span data-stu-id="e1c99-108">list</span></span>
- <span data-ttu-id="e1c99-109">圖書館</span><span class="sxs-lookup"><span data-stu-id="e1c99-109">library</span></span>

<span data-ttu-id="e1c99-110">此外，使用一些目前不支援的特定功能和自訂的清單，仍然會自動切換成傳統模式。</span><span class="sxs-lookup"><span data-stu-id="e1c99-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="e1c99-111">從2019年4月1日開始，停用租使用者層級的程式會退出現代清單，而文件庫會在5月 31 2019 日內開始並繼續執行。</span><span class="sxs-lookup"><span data-stu-id="e1c99-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="e1c99-112">由於承租人自願退出，以傳統模式表示的清單和文件庫會自動移至新式。</span><span class="sxs-lookup"><span data-stu-id="e1c99-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="e1c99-113">如果您需要傳統 [模式，請](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) 參閱此處的詳細資訊，並 PnP [在這裡](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) 描述您可以用來使用傳統模式體驗之選項及工具的 Powershell 說明。</span><span class="sxs-lookup"><span data-stu-id="e1c99-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
