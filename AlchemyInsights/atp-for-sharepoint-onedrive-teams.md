---
title: 適用於 SharePoint、OneDrive 及 Microsoft Teams 的 ATP
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712449"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="28020-102">適用於 SharePoint、OneDrive 及 Microsoft Teams 的 ATP</span><span class="sxs-lookup"><span data-stu-id="28020-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="28020-103">請遵循下列步驟來啟用高級威脅防護：</span><span class="sxs-lookup"><span data-stu-id="28020-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="28020-104">移至[https://protection.office.com](https://protection.office.com)並以全域管理員或安全性管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="28020-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="28020-105">在 [**威脅管理**] 底下的左側流覽窗格中，選擇 [**原則** \> **安全附件**]。</span><span class="sxs-lookup"><span data-stu-id="28020-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="28020-106">選取 **[開啟適用於 SharePoint、OneDrive 與 Microsoft Teams 的 ATP]**。</span><span class="sxs-lookup"><span data-stu-id="28020-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="28020-107">[建立活動警示原則](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts)，以在我們偵測到惡意檔時收到通知。</span><span class="sxs-lookup"><span data-stu-id="28020-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="28020-108">如需完整指示，請參閱本[主題](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="28020-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="28020-109">**附注**：依設計，ATP 不會掃描 SharePoint Online、商務 OneDrive 或 Microsoft 小組中的每一個檔案。</span><span class="sxs-lookup"><span data-stu-id="28020-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="28020-110">使用共用活動、訪客活動及威脅信號來識別惡意檔案的處理常式會以非同步方式掃描檔案。</span><span class="sxs-lookup"><span data-stu-id="28020-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="28020-111">如需詳細資訊，請參閱本[主題](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="28020-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
