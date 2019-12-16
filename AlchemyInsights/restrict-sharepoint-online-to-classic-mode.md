---
title: 限制 SharePoint Online 傳統模式
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048751"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8d718-102">限制 SharePoint Online 傳統模式</span><span class="sxs-lookup"><span data-stu-id="8d718-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8d718-103">有些組織還是需要傳統模式體驗。</span><span class="sxs-lookup"><span data-stu-id="8d718-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8d718-104">時沒有計劃来移除的細微層級的傳統模式，不會再可能會限制清單和文件庫的傳統模式整個組織 （承租人）。</span><span class="sxs-lookup"><span data-stu-id="8d718-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8d718-105">系統管理員將有下列選項來管理個別清單和文件庫的傳統模式使用我們提供下列層級的細微退出參數：</span><span class="sxs-lookup"><span data-stu-id="8d718-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="8d718-106">網站集合</span><span class="sxs-lookup"><span data-stu-id="8d718-106">site collection</span></span>
- <span data-ttu-id="8d718-107">網站</span><span class="sxs-lookup"><span data-stu-id="8d718-107">site</span></span>
- <span data-ttu-id="8d718-108">清單</span><span class="sxs-lookup"><span data-stu-id="8d718-108">list</span></span>
- <span data-ttu-id="8d718-109">文件庫</span><span class="sxs-lookup"><span data-stu-id="8d718-109">library</span></span>

<span data-ttu-id="8d718-110">此外，使用某些功能的清單及不支援的最新的自訂項目將仍會自動切換到傳統模式。</span><span class="sxs-lookup"><span data-stu-id="8d718-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8d718-111">開始 2019 年 4 月 1 日，若要停用租用戶層級的程序退出新式的清單和文件庫將會啟動並繼續執行 2019 5 月 31 日。</span><span class="sxs-lookup"><span data-stu-id="8d718-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="8d718-112">由於租用戶選擇不使用傳統模式中的文件庫與清單會自動將移至現代化。</span><span class="sxs-lookup"><span data-stu-id="8d718-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="8d718-113">如果您需要傳統模式的詳細資訊，請參閱[以下](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)和 PnP Powershell 指示[此處](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)所描述的選項和工具可用於目前使用傳統模式體驗。</span><span class="sxs-lookup"><span data-stu-id="8d718-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
