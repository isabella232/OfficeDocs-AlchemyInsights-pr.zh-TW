---
title: 螢幕畫面分享品質
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/26/2021
ms.locfileid: "52027302"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="0937a-102">螢幕畫面分享品質</span><span class="sxs-lookup"><span data-stu-id="0937a-102">Screen sharing quality</span></span>

<span data-ttu-id="0937a-103">在大部分情況下，螢幕畫面分享的品質問題，其根本原因是用戶端的頻寬有限。</span><span class="sxs-lookup"><span data-stu-id="0937a-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="0937a-104">在頻寬未受限的情況下，Teams 會最佳化媒體品質，包括最高 1080p 的視訊解析度、最高 30fps 的視訊和 15fps 的內容，以及高逼真度音訊。</span><span class="sxs-lookup"><span data-stu-id="0937a-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="0937a-105">Teams 在頻寬利用方面一向非常節約，可在低於 1.2 Mbps 的情況下提供 HD 視訊品質。</span><span class="sxs-lookup"><span data-stu-id="0937a-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="0937a-106">每個音訊/視訊通話或會議中的實際頻寬消耗，會因數個因素而有所不同，例如視訊配置、視訊解析度和每秒視訊畫面格數。</span><span class="sxs-lookup"><span data-stu-id="0937a-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="0937a-107">有更多頻寬可用時，品質和使用量便會增加，以提供最佳體驗。</span><span class="sxs-lookup"><span data-stu-id="0937a-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="0937a-108">下表說明 Teams 使用頻寬的方式：</span><span class="sxs-lookup"><span data-stu-id="0937a-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="0937a-109">**頻寬 (上傳/下載) 案例**</span><span class="sxs-lookup"><span data-stu-id="0937a-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="0937a-110">30 kbps 點對點音訊通話</span><span class="sxs-lookup"><span data-stu-id="0937a-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="0937a-111">130 kbps 點對點音訊通話和螢幕畫面分享</span><span class="sxs-lookup"><span data-stu-id="0937a-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="0937a-112">500 kbps 點對點品質視訊通話，360p，30fps</span><span class="sxs-lookup"><span data-stu-id="0937a-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="0937a-113">1.2 Mbps 點對點 HD 品質視訊通話，HD 720p 解析度，30fps</span><span class="sxs-lookup"><span data-stu-id="0937a-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="0937a-114">1.5 Mbps 點對點 HD 品質視訊通話，HD 1080p 解析度，30fps</span><span class="sxs-lookup"><span data-stu-id="0937a-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="0937a-115">500kbps/1Mbps 群組視訊通話</span><span class="sxs-lookup"><span data-stu-id="0937a-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="0937a-116">1Mbps/2Mbps HD 群組視訊通話 (1080p 螢幕上提供 540p 視訊)</span><span class="sxs-lookup"><span data-stu-id="0937a-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="0937a-117">如需詳細資訊，請參閱[針對 Microsoft Teams 準備組織的網路](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)。</span><span class="sxs-lookup"><span data-stu-id="0937a-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>